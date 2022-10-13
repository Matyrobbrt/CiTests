properties([pipelineTriggers([githubPush()])])

pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                echo "Hello there, you're running on branch ${sh(returnStdout: true, script: 'git rev-parse --abbrev-ref HEAD').trim()}"
            }
        }
    }
}