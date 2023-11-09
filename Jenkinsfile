pipeline{
    agent any
    stages{
        stage('Make directory'){
            steps{
                sh "mkdir ~/jenkins-test"

            post {
                failure {
                    echo 'some message'
                }
            }
            }
        }
        stage('make files'){
            steps{
                sh "touch ~/jenkins-test/file1"
            }
        }
    }
}
