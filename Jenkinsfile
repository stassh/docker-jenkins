pipeline {
    agent any
    stages {
        stage("Checkout") {
            steps {echo 'Checkout stage'}
        }

        stage("Verify Packages") {
            steps {
                echo 'Verify stage'
            }
        }

        stage("Build") {
            when {
                branch "master"
            }
            steps {
                echo 'Build stage'
            }
        }

        stage("Test") {
            when {
                branch "develop"
            }
            steps {
                echo 'Test stage'
            }
        }

        stage("Archive") {
            steps {
                sh 'cat ./Jenkisfile'
                echo 'Archive stage'

            }
        }
    }
}
