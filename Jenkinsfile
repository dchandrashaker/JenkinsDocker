pipeline {
    agent { dockerfile true }
    stages {
        stage (Build) {
            steps {
                docker build -t my_image .
                }
        }
    }
}
