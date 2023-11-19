pipeline {
    agent any
    option{
        buildDiscarder(logRotator(numToKeepStr: '1'))
    }
    triggers {
        pollSCM('* * * * *')
    }
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
