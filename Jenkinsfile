pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                script {
                    for (int i = 0; i<10; i++) {
                        echo("Loop ${i}")
                    }
                }
                sleep(5)
                echo "Start Build"
                sh("./mvnw clean compile test-compile")
                echo "Finish Build"
            }
        }
        stage("Test") {
            steps {
                echo "Test Running 1"
                echo "Test Running 2"
                sh("./mvnw test")
                echo "Test Running 3"
                echo "Test Running 4"
            }
        }
        stage("Deploy") {
            steps {
                echo "Deploy Running 1"
                echo "Deploy Running 2"
                echo "Deploy Running 3"
                echo "Deploy Running 4"
                sleep(20)
                echo "Deploy Running 5"
            }
        }
    }
    post {
        always {
            echo "Always Condition"
        }
        success {
            echo "Jika sukses"
        }
        failure {
            echo "Gagal tol"
        }
        cleanup {
            echo "gapeduli sukses or gagal kamu tetap yang terbaik"
        }
    }
}
