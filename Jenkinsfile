pipeline {
    agent any
    stages {
        stage('Sync Repos') {
            steps {
                sh """
                  git clone -b main git@github.com:ORG/A.git
                  cd A  
                  git remote add B git@github.com:ORG/B.git
                  git push B main
                """
            }
        }
    }
}
