pipeline {
    agent { docker { image 'ubuntu:latest' } }

    environment {
        GREETING = "Hello ${OWNER}"
        OWNER = "DMITRII"
    }

    stages {
        stage('sysinfo') {
            steps {
                sh "ls -la"
                sh "uname -a"
                echo "${GREETING} this is file from github"
            }
        }
    }
}
