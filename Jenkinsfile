pipeline {
 agent any
 parameters {
        string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I greet the world?')
    }
    stages {
        stage ('Compile Stage') {
             steps {
              echo "params greting: ${params.Greeting}"
                 echo "Build ID: ${env.BUILD_ID}"
                 echo 'Hello compile stage'
            }
        }
        stage ('Testing Stage') {
            steps {
             echo "params greting: ${params.chooseone}"
                echo "Jenkins URL: ${env.JENKINS_URL}"
                echo 'hello testing stage'
            }
        }
        stage ('Deployment Stage') {
            steps {
                echo "Job Name: ${env.JOB_NAME}"
                echo 'deploy stage'
            }
        }
        stage ('Clean up Stage') {
            steps {
                echo "Executor Number: ${env.EXECUTOR_NUMBER}"
                echo 'deploy stage'
            }
        }
        stage ('Finished Stage') {
            steps {
                echo "Wrok space: ${env.WORKSPACE}"
                echo 'deploy stage'
            }
        }
    }
}
