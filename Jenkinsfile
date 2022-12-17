pipeline {
    agent any

    stages {
        stage("build") {
            parallel {
                stage("windows") {
                    steps {
                        echo "building for windows..."
                    }
                }

                stage("linux") {
                    steps {
                        echo "building for linux..."
                    }
                }
            }
        }

        stage("test") {
            steps {
                echo "testing the application..."
            }
        }

        stage("deploy") {
            steps {
                echo "deploying the application...."
            }
        }
    }
}