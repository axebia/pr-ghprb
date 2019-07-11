node {  
    stage('Build') { 
           properties([[$class: 'GithubProjectProperty', displayName: '', projectUrlStr: 'https://github.com/axebia/pr-ghprb/']])
           properties([pipelineTriggers([<object of type org.jenkinsci.plugins.ghprb.GhprbTrigger>])])
    }
}
