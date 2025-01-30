pipeline {
    agent any

    stages {
        stage('clone git') {
            steps {
                // echo "Checkout the source code from the Git repository"
                git 'https://github.com/Shahakshar/jenkins.git'
            }
        }

        stage('Build') {
            steps {
                // echo "Execute build commands or scripts"
                //sh 'your-build-command-or-script.sh'
                python3 helloWorld.py
            }
        }

        stage('Test') {
            steps {
                echo "Execute test commands or scripts"
                //sh 'your-test-command-or-script.sh'
            }
        }

        stage('Staging') {
            steps {
                echo "Copy artifacts to a staging area (e.g., for further testing)"
                //sh 'cp -r build/* staging/'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploy artifacts to a production server or environment"
                //sh 'your-deployment-command-or-script.sh'
            }
        }

        stage('Monitor') {
            steps {
                echo "Perform monitoring and verification tasks"
                //sh 'your-monitoring-command-or-script.sh'
            }
        }
    }

    post {
        success {
            // This block executes if the pipeline is successful
            echo 'Deployment was successful!'
            // Add any additional success actions here
        }
        failure {
            // This block executes if the pipeline fails
            echo 'failed!'
            // Add any failure actions or notifications here
        }
    }
}   
