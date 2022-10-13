properties([pipelineTriggers([githubPush()])])

pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                checkout scm
                echo "Hello there, you're running on branch ${sh(returnStdout: true, script: 'git branch --show-current').trim()}"
            }
        }
    }
}