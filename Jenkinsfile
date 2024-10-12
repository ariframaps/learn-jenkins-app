pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'echo "hello world"'
            }
        }
    }
    //     stage('Build') {
    //         agent {
    //             docker {
    //                 image 'node: 18-alpine'
    //                 reuseNode true
    //             }
    //         }
    //         steps {
    //             sh '''
    //                 ls -la
    //                 node --version
    //                 npm --version
    //                 npm ci
    //                 npm run build
    //                 ls -la
    //             '''
    //         }
    //     }
    // }
}