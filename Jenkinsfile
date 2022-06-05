import java.text.SimpleDateFormat

pipeline {
    agent {
        label "demoAgent"
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }        
        stage('test') {
            steps {
                script {
                    def dateFormat = new SimpleDateFormat("yyMMddHHmm")
                    def date = new Date()
                    def TODAY = dateFormat.format(date)
                }
            }
        }
        stage('Print today') {
            steps {
                echo TODAY
            }
        }
    }
}
