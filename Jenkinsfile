pipeline{
    agent any

    stages{
        stage('Verify Branch'){
            steps{
<<<<<<< HEAD
                sh echo '$GIT_BRANCH'
=======
                sh(script: echo '$GIT_BRANCH')
>>>>>>> 455c2f2a1b058058d30e2cacab29d095074bd310
            }
        }

        stage('Docker Build'){
            steps{
                sh docker images -a
                sh(script: """
                    cd azure-vote/
                    docker images -a
                    docker build -t jenkins-pipeline .
                    docker images -a
                    cd ..
                """)
            }
        }
    }
}