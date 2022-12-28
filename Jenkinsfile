pipeline {
    agent none
    stages {
        stage('master build') {
            when {
                branch 'master'
            }
            steps {
               echo "Hello Master"
            }
        }
        stage('master-child build') {
            when {
                branch 'master-child'
            }
            steps {
               echo "Hello child"
            }
        }

    }
}
