// Nodejs

pipeline {
    agent { label 'WS' }
    stages {                                // Start of the stages
        stage('Lint Checks') {
            steps {
                sh "echo Installing JSLint"
                sh "npm i jslint"
                sh "node_modules/jslint/bin/jslint.js server.js"               
            }
        }
    }                                         // End of the stages
}