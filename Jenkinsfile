pipeline {
    agent any


    stages {
        stage('init') {
            steps {
                sh("echo 'hi'")
            }
        }
        stage('PR') {
            steps {
                script {
                    if (env.CHANGE_ID) {
                        echo pullRequest
                    }
                }
            }
        }
    }
}
