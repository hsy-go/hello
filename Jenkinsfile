pipeline {
    agent any
    def username = "Hsy"
    parameters {
        string(name: 'test', defaultValue: 'Hello', description: 'How should I greet the world?')
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo "hellow ${username}"
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
