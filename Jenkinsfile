pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'usernamepassword', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')]) {
                    sh '''
                        echo "Username: $USERNAME"
                    '''
                }
            }
        }
    }
}
