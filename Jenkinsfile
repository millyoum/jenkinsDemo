import java.text.SimpleDateFormat

pipeline {
    agent {
        label "demoAgent"
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
