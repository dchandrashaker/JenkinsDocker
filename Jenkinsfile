pipeline {
    agent { dockerfile true }
    stages {
        stage (Build) {
            steps {
                docker build -t Alpine_GIT_image .
                }
        }
    }
}
