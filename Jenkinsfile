pipeline {
    agent any
    stages {
        stage('Make directory') {
            steps {
                script {
                    try {
                        sh "mkdir ~/jenkins-test"
                    } catch (Exception e) {
                        echo "Failed to make directory"
                    }
                }
            }
        }
        stage('make files') {
            steps {
                sh "touch ~/jenkins-test/file1"
            }
        }
    }
}
