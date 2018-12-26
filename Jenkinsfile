pipeline {
    agent any
    //String TOMCAT_DIR 'E:\\softwares\\apache-tomcat-8.5.37\\webapps'
    stages {
        stage('Build')
        {
            steps {
                sh 'echo "**** BUILD STARTED ****"'
                bat 'mvn clean install' 
            }
        }
        stage('Deploy')
        {
            steps {
                sh 'echo "Deploying to TOMCAT'
                sh 'echo E:\\softwares\\apache-tomcat-8.5.37\\webapps'
                sh 'copy target/JenkinsWar.war E:\\softwares\\apache-tomcat-8.5.37\\webapps'
            }
        }
    }
}
