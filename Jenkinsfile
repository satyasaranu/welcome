pipeline {
    agent any
    
    tools {
        maven 'maven-3.6.0'
    }
    stages {
        stage(pullgit) {
            steps {
            git 'https://github.com/satyasaranu/welcome.git'
            }
        }
        
        stage(build) {
            steps {
                sh "mvn package"
            }
        }
        stage(deploy) {
            steps {
                sh "echo deploy to nexus"
            }
        }
    }
}