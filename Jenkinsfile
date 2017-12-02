pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                bat 'cd git-example ; bat ./build' 
            }
        }
        stage('Test'){
            steps {
                bat 'cd git-example ; bat ./test'
            }
        }
        stage('Deploy') {
            steps {
                bat 'echo "Deploy..."'
            }
        }
    }
}
