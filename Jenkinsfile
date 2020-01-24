pipeline {
        agent any
        stages {
            stage('clone') {
                steps {
                    sh "rm -rf *"
                    git credentialsId: '59f55a83-9d3f-4d4e-8397-cf5dacb5be96', url: 'https://github.com/Folio68/test.git'  sh "rm -rf *"
                }
            stage('build') {
                steps {
                sh "cd jenkins/ && javac Main.java"
                }
            stage('run') {
                steps {
                sh "cd jenkins/ && java Main""
                }
            }
}
