pipeline {
    agent any
    triggers {
    pollSCM('* * * * *')
    }
    environment{
        repo_name = 'front'
    }
    stages {
        stage('build') {
            steps {
            git url: 'https://github.com/Mehrdad-Farshi/front.git', branch: 'master'
            echo "repo name : ${repo_name} BUILD ID : ${env.BUILD_ID}, JENKINS URL : ${env.JENKINS_URL}"
            sh 'pwd'
            sh 'ls'
            }
        }
    }
}