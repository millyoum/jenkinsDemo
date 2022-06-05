import java.text.SimpleDateFormat

pipeline {
    agent {
        label "demoAgent"
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building.'
            }
        }       
 
        stage('get date and time') {
            steps {
                script {
                    def dateFormat = new SimpleDateFormat("yyMMddHHmm")
                    def date = new Date()
                    Today = dateFormat.format(date)
                }
            }
        }
        stage('Print today') {
            steps {
                echo Today
            }
        }
    }
}
