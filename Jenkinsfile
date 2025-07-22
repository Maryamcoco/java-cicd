pipeline{
    agent any
    tools{
        maven 'Maven_3_9_10'
    }
    stages{
        stage('build'){
            steps{
                sh "mvn clean install -DskipTest"
                echo "Build Success"
            }
        }

        stage('Test'){
            steps{
                sh "mvn test"
                echo "test success"
            }
        }

        stage('Package'){
            steps{
                sh "mv package"
                echo "package success"  
            }
        }
    }
}
