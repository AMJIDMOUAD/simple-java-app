node {
    stage('Checkout') {
        checkout scm: [
            $class: 'GitSCM',
            branches: [[name: 'declarativepip']],
            userRemoteConfigs: [[url: 'https://github.com/AMJIDMOUAD/simple-java-app.git']]
        ]
    }

    stage('Build') {
        sh 'echo "Building..."'
    }
    stage('Test') {
        sh 'echo "Testing..."'
    }
    stage('Deploy') {
        sh 'echo "Branch is ${env.BRANCH_NAME}"'
    }
}
