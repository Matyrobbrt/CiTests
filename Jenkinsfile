properties([pipelineTriggers([githubPush()])])

pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                checkout scm
                echo "Hello there, you're running on branch ${env.BRANCH_NAME}"
            }
        }
        stage('tag_stuff') {
            when { tag '*' }
            steps {
                echo "Hello there, you're running on tag ${env.BRANCH_NAME}"
            }
        }
    }
}