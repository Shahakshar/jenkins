pipeline {
    agent any

    stages {
        stage('clone git') {
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
stage('Ansible Deployment') {
             steps {
                    ansible-playbook installation: 'Ansible', playbook: 'deploy-playbook.yml'
             }
         }
