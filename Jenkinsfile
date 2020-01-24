pipeline {
        agent any
        stages {
            stage('Clone') {
                steps {
                    sh "rm -rf *"
                    git credentialsId: '59f55a83-9d3f-4d4e-8397-cf5dacb5be96', url: 'https://github.com/Folio68/test.git'
                }
            }
            stage('Build') {
                steps {
                sh "javac Main.java"
                }
            }
            stage('Run') {
                steps {
                sh "java Main"
                }
            }
        }
}
