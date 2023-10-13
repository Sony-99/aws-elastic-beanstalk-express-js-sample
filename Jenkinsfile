pipeline {
    agent any
    stages {

        stage('Clone the code') {
            steps {
                echo "Cloning the repo"
                git url: "https://github.com/Sony-99/aws-elastic-beanstalk-express-js-sample.git", branch: "main"            }
        }       
        
        stage('Build the code') {
            steps {
                echo "Building the image"
                sh "docker build -t my-node-app ."
            }
        }
    }
}

