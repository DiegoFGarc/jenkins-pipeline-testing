pipeline {
    agent any

    environment {
  		F_VAR = credentials('first-variable')
    }

    stages {
        stage('Build') {
            steps {
                sh '''
			            sh 'echo "Building..."'
			            sh 'echo $F_VAR'
           
                    '''  
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Running tests..."'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying..."'
            }
        }
    }
}
