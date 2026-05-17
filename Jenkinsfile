pipeline {

    agent {

        kubernetes {

            yaml """

apiVersion: v1
kind: Pod

spec:

  containers:

    - name: jnlp

      image: jenkins/inbound-agent:latest

      tty: true

"""
        }
    }

    stages {

        stage('Build') {

            steps {

                sh 'echo payment service pipeline running'
            }
        }
    }
}