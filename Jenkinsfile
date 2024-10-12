pipeline {
    agent any 

    stages {
        stage('Build') {
            agent {
                docker {
                    image 'node: 18-alpine'
                    image 'alpine/git' // Menggunakan image Alpine dengan Git
                    reuseNode true
                }
            }
            steps {
                sh '''
                    ls -la
                    node --version
                    npm --version
                    npm ci
                    npm run build
                    ls -la
                '''
            }
        }
    }
    
}