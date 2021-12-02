pipeline {
    agent{
        docker{
            image '3.8.4-jdk-8'
        }
    }
    stages{
        stage('Build'){
            steps{
                sh 'mvn -B -DskipTests clean package'
            }
        }
        stage('Test'){
             steps{
                sh 'mvn test'
             }
        }
        stage('QA'){
            steps{
                echo 'QA'
            }
        }
    }
}