pipeline {
    agent any
    stages {
        stage("Compile Stage") {
            steps {
                withGradle() {
                    sh 'gradle clean compile'
                }
            }
        }
        stage("Build Stage") {
            steps {
                withGradle() {
                    sh 'gradle clean build'
                }
            }
        }
    }
}