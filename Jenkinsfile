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
                sh "ls -l"   // List files in workspace
                sh "pwd"     // Print working directory
            }
        }
        stage('Run Python Script') {
            steps {
                sh "python3 helloworld.py" // this fine
                sh "python3 Prog1.py" // this what it is
            }
        }
    } 
}
