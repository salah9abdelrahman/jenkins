pipeline {
    agent any
    stages {
        stage('Run frontend') {
            steps {
                echo 'executing yarn start...'
                nodejs('NodeJS-24'){
                    sh 'yarn install'
                }
            }
        }

        stage('Run backend') {
            steps {
                echo 'executing gradle run...'
                gradle{
                    sh 'gradle run'
                }
            }
        }
    }
}