pipeline {
    agent any
    stages {
        stage('Clone Repo') {
            steps {
                git branch: 'main', url: 'https://github.com/PillaiSathya/Git_Assignment.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the project...'
            }
        }
        stage('Archive Artifact') {
            steps {
                archiveArtifacts artifacts: '**/*.jar', fingerprint: true
            }
        }
    }
}
