pipeline {
    agent any

    triggers {
        githubPush()
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "Building application..."
                // example:
                // npm install
                // mvn clean package
                // docker build -t myapp .
            }
        }

        stage('Run / Test') {
            steps {
                echo "Running application or tests..."
            }
        }
    }
}
