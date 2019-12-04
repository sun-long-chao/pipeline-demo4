pipeline {
    agent any
    stages {
        stage('Non-Sequential Stage') {
            steps {
                println "On Non-Sequential Stage"
            }
        }
        stage('Sequential') {
            environment {
                FOR_SEQUENTIAL = "some-value"
            }
            stages {
               stage('In Sequential 1') {
                   steps {
                       println "In Sequential 1"
                   }
               }
               stage('In Sequential 2') {
                   steps {
                       println "In Sequential 2"
                   }
               }
            }
        }
    }
}