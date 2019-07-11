pipeline {
    agent any
    stages {
        stage('Git Clone') {
            steps {
                git credentialsId: 'xebia_github', url: 'https://github.com/axebia/simple-grable-build.git'
            }
        }
        stage('Gradle Build and Deploy') {
            steps {
                properties([[$class: 'GithubProjectProperty', displayName: '', projectUrlStr: 'https://github.com/axebia/pr-ghprb/']])
            properties([pipelineTriggers([<object of type org.jenkinsci.plugins.ghprb.GhprbTrigger>])])
            }  
    }
}
}
