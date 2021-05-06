@Library('multibranchlibrary') _

pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                script{
                    isBuildReplay()
                }
            }
        }
    }
}
