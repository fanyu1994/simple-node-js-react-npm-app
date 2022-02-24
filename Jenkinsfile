pipeline {
    agent any
    stages {
        stage('Build') {
            steps {  // window 使用 bat， linux 使用 sh
                sh 'npm i'
                sh 'npm run build'
            }
        }
    }
}
