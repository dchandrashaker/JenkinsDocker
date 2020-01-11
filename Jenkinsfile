pipeline {
    agent { dockerfile true }
    stages {
        stage (Build) {
            steps {
                docker build -t nginx_image .
                }
                }
        stage('Test') {{
            steps {
                docker images
                mkdir -p /webroot
                docker run -d -v /webroot:/var/www/html -p 80:80 --name hakase nginx_image
                docker ps
            }
        }
        }
    }
}
