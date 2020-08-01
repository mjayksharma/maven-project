pipeline{
    agent{
        label "Master"
    }
    stages{
        stage("mjay_stage1"){
            steps{
                echo "========executing mjay_stage1========"
                git 'https://github.com/mjayksharma/maven-project.git'
            }
            post{
                always{
                    echo "========always========"
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
