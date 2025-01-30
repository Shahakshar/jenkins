pipeline { 
    agent any
    stages {
        stage('Clone Git') {
            steps {
                git 'https://github.com/Shahakshar/jenkins.git'
            }
        }
        stage('Build Code') {
            steps {
                sh "chmod u+x Prog1.py"
                sh "./Prog1.py"
                sh "chmod u+x helloworld.py"
                sh "./helloworld.py"
            }
        }
        
    } 
}
