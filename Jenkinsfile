pipeline {
    agent any
    stages {
        stage("hello") {
            steps {
                echo("Hello World") 
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
