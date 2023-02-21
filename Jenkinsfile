pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ PES2UG20CS189-1.cpp -o PES2UG20CS189-1'
            }
        }
        stage('Test') {
            steps {
                sh './PES2UG20CS189-1'
            }
        }
        stage('Deploy') {
            steps {
                sh './PES2UG20CS189-1'
            }
        }
    }
    post {
        always {
            script {
                if (currentBuild.result == "FAILURE") {
                    echo "Pipeline failed"
                }
            }
        }
    }
}


