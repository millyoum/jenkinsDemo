pipeline {
    agent {
        label "Built-In Node"
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                build 'SeleniumMaven'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....!!!'
            }
        }
    }
}
