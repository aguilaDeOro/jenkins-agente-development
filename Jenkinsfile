pipeline {
   
    agent{
        node {
            label 'production-c'
        }
    }
    stages {
        stage('Build') {
            steps {
            
                echo "Building ... in the node ${NODE_NAME}  and in the executor ${EXECUTOR_NUMBER}"
                sh 'uname -n'
            }
        }
        stage('Test') {
            steps {
              echo "Testing ... in the node ${NODE_NAME}  and in the executor ${EXECUTOR_NUMBER}"
              sh 'uname -n'
            }
        }
        stage('Deploy') {
            steps {
             echo "Deploying ... in the node ${NODE_NAME}  and in the executor ${EXECUTOR_NUMBER}"  
             sh 'uname -n'
            }  
        }
    }
    post {
        always {
            echo 'Pipeline terminado...'
        }
        success {
            echo 'completado con exito.'
        }
        failure {
            echo 'completado con errores.'
        }
    }
}
