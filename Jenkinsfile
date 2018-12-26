pipeline {
    agent any
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
                bat 'echo "Done! Now get some docker or server to deploy"'
            }
        }
    }
}
