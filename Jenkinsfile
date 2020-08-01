pipeline{
    agent{
        label "master"
    }
    stages{
        stage("mjay_stage1"){
            steps{
                echo "========executing mjay_stage1========"
                sh 'echo Hello bhai'
                git 'https://github.com/mjayksharma/maven-project.git'
            }
        }
    }
}
