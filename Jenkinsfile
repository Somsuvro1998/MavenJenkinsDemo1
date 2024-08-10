pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build App'
            }
        }
        stage('Test') {
            steps {
                echo 'Test App'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy App'
            }
        }
        
    }
    post{
        always{
            emailext body: 'please find the pipeline at http://localhost:8080/job/Pipeline2/', subject: 'Pipeline Status', to: 'palz.somsuvro@gmail.com'
        }
    }
}
