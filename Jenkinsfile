pipeline {
    agent any

    options {
        // Define options if needed
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // Add your build commands here
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                // Add your test commands here
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add your deployment commands here
            }
        }
    }

    // Specify the branch in the SCM configuration
    options {
        skipDefaultCheckout(true)
    }

    // Define the checkout step with the specific branch
    stages {
        stage('Checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: 'main']], userRemoteConfigs: [[url: 'https://github.com/harshada-zurunge/Jenkins_demo.git']]])
            }
        }
    }
}
