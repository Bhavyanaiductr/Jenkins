pipeline {
    agent any 
    stages {
        stage('SCM') {
            steps {
                echo 'Hello world!' 
                sh '''
                echo "Now it is going to clone the code from github"
                git clone https://github.com/Bhavyanaiductr/Testing_Project.git
                echo "clonind is done"
                mvn clean
                mvn compile
                mvn package
                '''
            }
        }
        stage('BUILD'){
            steps {
                echo 'This is build stage'
                
            }
        }
        stage('BACKUP') {
            steps {
                echo 'this is backup stage'
            }
        }
    }
}
