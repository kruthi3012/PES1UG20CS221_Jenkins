pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES1UG20CS221-5 new.cpp'
            }
        }
        
        stage('Test') {
            steps {
                sh './PES1UG20CS221-5'
            }
        }
    }
    post{
        failure{
            echo 'Pipeline failed'
        }
    }
}
