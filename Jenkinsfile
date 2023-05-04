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
            environment {
  		        S_VAR = "Segunda variable"
            }
            steps {
                sh 'echo "Hello, ${S_VAR}!"'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying..."'
            }
        }
    }
}
