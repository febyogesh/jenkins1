pipeline{
    agent any
    environment{
        PYTHON="C:\\Python313\\python.exe"
    }
    
    stages{
        stage("checkout code"){
            step{
             checkout scm
            }
        }
        stage("extract data"){
            step{
             bat "${evn.PYTHON} extract.py"
            }
        }
    }
}