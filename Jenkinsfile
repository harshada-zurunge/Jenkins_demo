pipeline {
    agent any
    
    environment {
        GITHUB_CREDENTIALS = credentials('bb17d395-b3ef-4709-97bc-0e2901fe0493')
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

