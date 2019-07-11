pipeline {
    agent any
    stages {
        stage('Git Clone') {
            steps {
                git credentialsId: 'xebia_github', url: 'https://github.com/axebia/simple-grable-build.git'
            }
        }
        stage('Github Project') {
            steps {
            properties([
  parameters([
    string($class: 'GithubProjectProperty', displayName: '', projectUrlStr:'https://github.com/axebia/pr-ghprb/' )
  ])
])
            }  
    }
}
}
