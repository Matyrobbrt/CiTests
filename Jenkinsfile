properties([pipelineTriggers([githubPush()])])

pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                echo "Hello there: ${env.BRANCH_NAME}"
            }
        }
    }
}