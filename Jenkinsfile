pipeline {
    agent any
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
