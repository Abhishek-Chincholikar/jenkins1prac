pipeline {
    agent any

    stages {
        stage('Fetch') {
            steps {
                echo 'Fetching from Repo'
                git 'https://github.com/Abhishek-Chincholikar/jenkins1prac.git'
            }
        }
        stage('build') {
            steps {
                echo 'Building the program '
                bat 'javac Hello.java'
            }
        }
        stage('Execute') {
            steps {
                echo 'Exectuing the program...'
                bat 'java Hello'
        }
    }
}
        post{
            success{
                echo'Pipeline built Successfully'
            }
            failure{
                echo'Pipeline failed'
            }
        }
    }
