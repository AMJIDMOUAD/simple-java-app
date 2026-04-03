node {

    git branch: 'declarativepip', url: 'https://github.com/AMJIDMOUAD/simple-java-app.git'

    stage('Build') {
        sh 'echo "Building..."'
    }
    stage('Test') {
        sh 'echo "Testing..."'
    }
    stage('Deploy') {
        script {
            if (env.BRANCH_NAME == 'master') {
                sh 'echo "Deploying to production..."'
            } else {
                sh 'echo "Deploying to :${env.BRANCH_NAME}..."'
            }
        }
    }
}