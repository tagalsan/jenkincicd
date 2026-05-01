pipeline{
    agent any
    environment{
        PYTHON = 'C:\\Users\\Sanket\\AppData\\Local\\Programs\\Python\\Python313\\python.exe'
    }
    stages{
        stage ('checkout code'){
            steps {
                checkout scm
            }
        }
        stage ('show python version'){
            steps{
                bat "${env.PYTHON} --version"
            }

        }
        stage ('Run extract.py'){
            steps{
                bat "${env.PYTHON} extract.py"
            }

        }
    }
}