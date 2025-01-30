pipeline { 
    agent any
    stages {
        stage('Clone Git') {
            steps {
                sh "rm -rf *"  // Clean workspace to avoid caching issues
                git 'https://github.com/Shahakshar/jenkins.git'
                sh "ls -l"     // Check if files were cloned
            }
        }
        stage('Check Files') {
            steps {
                sh "ls -l"   // List files in workspace
                sh "pwd"     // Print working directory
            }
        }
        
    } 
}
