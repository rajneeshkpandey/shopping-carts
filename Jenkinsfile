pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       maven 'maven' 
    }
    

    stages{
        stage('build-the-app-bycode'){
            steps{
                echo 'this is the build job'
                sh 'compile'
            }
        }
        stage('test-the-app-bycode'){
            steps{
                echo 'this is the test job'
                sh 'clean test'
            }
        }
        stage('pacakage-the-app-bycode'){
            steps{
                echo 'this is the package job'
                sh 'package'
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...by Rajneesh'
        }
        
    }
    
}
