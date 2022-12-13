pipeline {
    agent any
    tools {
        maven 'maven 3.8.6'
    }

    stages {
        stage('PULL') {
            steps {
                git branch: 'main', url: 'https://github.com/sachinayyar/php-sample.git'
            }
        }
        stage('BUILD') 
        {
            steps 
            {
                echo 'building'
                
            }
        }
        stage('CREATE IMAGE') 
        {
            steps 
            {
                echo 'creating'
                
            }
        }
        stage('DEPLOY') 
        {
            steps 
            {
                echo 'deploying'
                
            }
        }
    }
}
