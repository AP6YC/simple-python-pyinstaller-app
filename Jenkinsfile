pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                docker {
                    image 'python:2-alpine' 
                }
            }
            steps {
                bash 'python -m py_compile sources/add2vals.py sources/calc.py' 
            }
        }
    }
}