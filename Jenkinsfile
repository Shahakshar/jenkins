pipeline {
    agent any

    stages {
        stage('Clone git') {
            steps {
                // echo "Checkout the source code from the Git repository"
                git 'https://github.com/Shahakshar/jenkins.git'
            }
        }

        stage('Build code') {
            steps {
                // echo "Execute build commands or scripts"
                //sh 'your-build-command-or-script.sh'
                python3 helloWorld.py
            }
        }
    }
}  
