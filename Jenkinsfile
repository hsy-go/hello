pipeline {
    agent any
    parameters {
        string(name: 'test', defaultValue: 'Hello', description: 'How should I greet the world?')
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                script {
                    def username="Hsy"
                    echo "hellow ${username}"
                }
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                echo "parameters ${parameters.test}"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
