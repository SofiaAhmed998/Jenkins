pipeline {
    agent any
    
    stages {
        stage('Delete Old Cloned Repository') {
            steps {
                deleteDir()
            }
        }
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/SofiaAhmed998/ToCS.git'
            }
        }
        stage('Build') {
            steps { 
                bat 'MyWorld.py'
            }
        }
    }
}
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Allication build stage...' 
        }
       }
        stage('Test') {
            steps {
                echo 'Allication test stage' 
        }
        }
        stage('Run') {
            steps {
                echo 'Allication run stage' 
            }
        }
    }
}
