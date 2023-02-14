pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ -c main/PES1UG20CS649.cpp'
                sh 'g++ -o PES1UG20CS629 main/PES1UG20CS649.cpp'
                echo 'build stage successfull'
            }
        }
        stage('Test'){
            steps{
                sh './main/PES1UG20CS649'
                echo 'test stage successful'
            }
        }
        stage('Deploy'){
            steps{
                echo 'Deployment Successful'
            }
        }
    }
    post{
        failure{
            echo 'Pipeline Failed'
        }
    }
}
