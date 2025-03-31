pipeline {
    agent any
    stages {
        stage('Build Angular App') {
            when {
                changeset '**/angular-app/**' // Build an angular app
            }
            steps {
                echo 'Building an angular app is ongoing...'
                sh 'cd angular-app && npm install && npm run build'
            }
        } stage('Build React App') {
            when {
                changeset '**/react-app/**' // Build an react app
            }
            steps {
                echo 'Building an react app is ongoing...'
                sh 'cd react-app && npm install && npm run build'
            }
        } stage('Build Vue App') {
            when {
                changeset '**/vue-app/**' // Build a vue app
            }
            steps {
                echo 'Building an vue app is ongoing...'
                sh 'cd vue-app && npm install && npm run build'
            }
        }
    }
}
