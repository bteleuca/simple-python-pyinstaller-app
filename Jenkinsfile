pipeline {
    agent { label 'viyahost' }
    stages {
        stage('Build') { 
            agent { docker 'python:2-alpine' }
            steps {
                sh 'python -m py_compile sources/add2vals.py sources/calc.py' 
            }
        }
    }
}
