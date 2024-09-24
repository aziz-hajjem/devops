pipeline {
    agent any
    tools {
        maven 'M2_HOME'
    }
    stages {
        stage('GIT') {
            steps {
                git branch : 'master',
                url :'https://github.com/aziz-hajjem/atelier_devops.git'
            }
        }
        stage('Compile') {
            steps {
                sh 'mvn compile';
            }
        }
    }
}
