pipeline {
 agent any
    stages {
        stage ('Compile Stage') {
             steps {
                 echo "Build ID: ${env.BUILD_ID}"
                 echo 'Hello compile stage'
            }
        }
        stage ('Testing Stage') {
            steps {
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
