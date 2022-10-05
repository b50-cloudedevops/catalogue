pipeline {
    agent any
    stages {
        stage('Installing the node js dependencies') {
            steps {
                sh "npm install"
            }
        }
        stage('Lint checks') {
            steps {
                sh "echo installing jslint"
                sh "npm i jslint"
                sh "~/node_modules/jslint/bin/jslint.js server.js"
            }

        }
    }
}