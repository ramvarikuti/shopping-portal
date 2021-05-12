pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
   Tools{
nodejs ‘nodejs’        

    }
   

    stages{
        stage('build'){
            steps{
                echo 'this is the build job'
                sh 'npm install'
            }
        }
        stage('test'){
            steps{
                echo 'this is the test job'
                sh 'npm test'
                //sleep 9
            }
        }
        stage('package'){
            steps{
                echo 'this is the package job'
                sh ‘npm run package'
                //sleep 7
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}

