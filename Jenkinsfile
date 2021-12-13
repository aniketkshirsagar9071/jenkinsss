pipeline{
    agent any
    stages{
        stage("my-project"){
            steps{
                echo "my first jenkins project"
                sh 'ls'
            }
            post{
                always{
                    echo "this is ci-cd project"
                }
                success{
                    echo "========A executed successfully========"
                }
                failure{
                    echo "========A execution failed========"
                }
            }
        }
    }
    post{
        always{
            echo "========always========"
        }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    }
}
