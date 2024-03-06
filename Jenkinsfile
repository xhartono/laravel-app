pipeline{
    agent{
        label "node"
    }
    stages{
        stage("Stage 1"){
            steps{
                echo "========Stage 1========"
            }
            post{
                always{
                    echo "========always========"
                }
                success{
                    echo "========Stage 1 executed successfully========"
                }
                failure{
                    echo "========Stage 1 execution failed========"
                }
            }
        }
        stage("Stage 2"){
            steps{
                echo "========Stage 2========"
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