properties([pipelineTriggers([githubPush()])])

pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                echo "Hello there: ${org.jenkinsci.plugins.workflow.cps.EnvActionImpl.class.getMethod('getOverriddenEnvironment').invoke(env)}"
            }
        }
    }
}