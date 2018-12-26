pipeline {
    agent any
    def TOMCAT_DIR = 'E:\\softwares\\apache-tomcat-8.5.37\\webapps'
    stages {
        stage('Build')
        {
            steps {
                bat 'echo "**** BUILD STARTED ****"'
                bat 'mvn clean install' 
            }
        }
        stage('Deploy')
        {
            steps {
                bat 'echo "Deploying to TOMCAT'
                bat 'echo ${TOMCAT_DIR}'
                bat 'xcopy target\\JenkinsWar.war ${TOMCAT_DIR}'
            }
        }
    }
}
