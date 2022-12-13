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
                script {
                    openshift.withCluster() {
                        openshift.withProject ("cicd")
                        {
                            openshift.newBuild("--name=cicd","--docker-image=registry.redhat.io/rhel8/php-74","binary")
                        }
                    }
                }  
                
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
