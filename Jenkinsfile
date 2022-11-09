pipeline {
    agent any
    tools {
        maven "Admin"
    }
    stages {
        stage('Checkout') {
            steps {
                // Get some code from a GitHub repository
                git url: 'https://github.com/Gifty147/Jenkinsclass.git', 
                    branch: 'Jenkinsclass',
                    credentialsId: '97ba5c35-497e-45c0-884e-635bdb4afb60'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
            } 
        }   
    }
}