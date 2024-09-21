pipeline {
    agent any
    options {
        disableConcurrentBuilds()
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
