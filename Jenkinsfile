pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       npm 'npm' 
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
                sh 'npm install'
                sh 'npm test'
            }
        }
        stage('package'){
            steps{
                echo 'this is the package job'
                sh 'npm install'
                sh 'npm run package'
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}
