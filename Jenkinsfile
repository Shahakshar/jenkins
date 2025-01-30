pipeline { 
    agent any
    stages {
        stage('Clone Git') {
            steps {
                git branch: 'main', url: 'https://github.com/Shahakshar/jenkins.git'
            }
        }
        stage('Check Files') {
            steps {
                sh "ls -l"   
                sh "pwd"     
            }
        }
        stage('Run Python Script') {
            steps {
                sh "python3 helloworld.py" 
                sh "python3 Prog1.py" 
            }
        }
    } 
}
