pipeline {
    agent any
    
    environment {
        GITHUB_CREDENTIALS = credentials('harshada-zurunge')
    }

    stages {
        stage('Checkout') {
            steps {
                script {
                    checkout([$class: 'GitSCM', branches: [[name: '*/main']], userRemoteConfigs: [[url: 'https://github.com/harshada-zurunge/Jenkins_demo.git', credentialsId: env.GITHUB_CREDENTIALS]]])
                }
            }
        }

        // Add more stages as needed
    }
}

