pipeline {
    agent any

    environment {
  		F_VAR = credentials('first-variable')
    }

    stages {
        stage('Build') {
            steps {
                sh '''
			            echo "Building..."
			            echo $F_VAR
           
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
