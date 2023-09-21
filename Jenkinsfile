pipeline {
    agent any
    stages {
        stage ('CheckOut Git'){
            steps{
                
                echo 'Pulling ...';
                git branch: 'master',
                url : 'https://github.com/youssefbenfraj/avec-maven.git';
            }
        }
        stage ('Testing Maven'){
            steps{
                sh """mvn -version"""
            }
        }
    }
}
