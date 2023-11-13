
pipeline{

  agent any

  stages{

    stage('Build'){

      steps{

        sh 'echo "Building"'
        sh 'ls -l'

      }

    }

    stage('Test'){

      steps{

        sh 'echo "Testing 1 2 3 4"'
        sh 'pwd'
        sh 'touch testfile.txt'
        sh 'ls -l'

      }

    }

    stage('Deploy'){
        steps{
            sh 'cat ./deploy.sh'
            sh 'echo "Deploying..."'
            sh 'mv testfile.txt /tmp'
            sh 'ls -l /tmp'
        }

    }

 }
}