pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       Maven 'maven' 
    }
    

    stages{
        stage('build-the-app-bycode'){
            steps{
                echo 'this is the build job'
                mvn 'compile'
            }
        }
        stage('test-the-app-bycode'){
            steps{
                echo 'this is the test job'
                mvn 'clean test'
            }
        }
        stage('pacakage-the-app-bycode'){
            steps{
                echo 'this is the package job'
                mvn 'package'
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...by Rajneesh'
        }
        
    }
    
}
