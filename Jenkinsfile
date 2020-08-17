pipeline {
    agent { dockerfile true }
    stages {
        stage (Build) {
            steps {
                docker build -t dchandrashaker/my_image .
                }
        }
    }
}
