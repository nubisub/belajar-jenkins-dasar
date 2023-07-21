pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                echo "Build Running"
            }
        }
        stage("Test") {
            steps {
                echo "Test Running"
            }
        }
        stage("Deploy") {
            steps {
                echo "Deploy Running"
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