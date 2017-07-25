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
             echo "params Choose one: ${params.'choose one'}"
                echo "Jenkins URL: ${env.JENKINS_URL}"
                echo 'hello testing stage'
            }
        }
        stage ('Deployment Stage') {
            steps {
                mail to: 'team@example.com', subject: 'The Pipeline failed :(', body: 'what should i say'
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
