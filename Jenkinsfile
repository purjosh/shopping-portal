pipeline{
    agent any
// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs' 
    }
    
    stages{
        stage('build'){
            steps{
                echo 'this is the Build job'
                sh 'npn install'
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'npn test'
            }
        }
        stage('package'){
            steps{
                echo 'this is the package job'
                sh 'npn run package'
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}

