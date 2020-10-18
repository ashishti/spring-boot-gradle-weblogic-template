pipeline {
    agent any
    stages {
        stage("Compile Stage") {
            steps {
                withGradle(gradle: 'gradle-6.7') {
                    sh 'gradle clean compile'
                }
            }
        }
        stage("Build Stage") {
            steps {
                withGradle(gradle: 'gradle-6.7') {
                    sh 'gradle clean build'
                }
            }
        }
    }
}
