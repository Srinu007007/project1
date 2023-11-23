pipeline {
    agent any

    stages {
        stage('chekcout') {
            steps {
                git 'https://github.com/Srinu007007/project1.git'
                echo 'check out'
            }
        }
        stage('Test') {
            steps {
                bat 'mvn test'
                echo 'test project'
            }
        }
        stage('Deploy') {
            steps {
                bat 'mvn verify'
                echo 'Deploy project'
            }
        }
    }
}
