#!/usr/bin/env groovy
properties([
  pipelineTriggers([
    upstream(
      threshold: 'SUCCESS',
      upstreamProjects: 'https://github.com/Sireddy669/sireddy2.git'
    )
  ])
])

pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                sh 'pwd' 
            }
        }
        stage('Test'){
            steps {
                sh 'java -version'
                
            }
        }
        stage('Deploy') {
            steps {
                sh 'ls'
                sh 'pwd'
              
              agent any

    parameters {
        booleanParam(defaultValue: true, description: '', name: 'userFlag')
    }

    stages {
        stage("foo") {
            steps {
                echo "flag: ${params.userFlag}"
            }
            }
            }
        }
    }
}
