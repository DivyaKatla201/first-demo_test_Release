pipeline {
    agent any
    options {
        disableConcurrentBuilds()
    }
    environment {
        WORKSPACE = '/opt/jenkins-workspace/workspace/project-demo'
    }
    stages {
        stage('parallel execution') {
                    steps {
                            echo 'cloning repo'
                            git 'https://github.com/kalyanreddyc/first-demo.git'
                    }
                }
                stage('build') {
                    steps {
                            sh """
                            mvn clean package
                            """
                    }
                }
                
        }
        
}
