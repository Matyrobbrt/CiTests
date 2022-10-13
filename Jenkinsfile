properties([pipelineTriggers([githubPush()])])

pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                def branch = sh(returnStdout: true, script: 'git rev-parse --abbrev-ref HEAD').trim()
                echo "Hello there, you're running on branch $branch"
            }
        }
    }
}