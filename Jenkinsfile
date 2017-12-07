#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: 'Sireddy1',
    projectUrlStr: 'https://github.com/Sireddy669/sireddy1.git/'],
    pipelineTriggers([
      upstream(upstreamProjects: "https://github.com/Sireddy669/sireddy2.git/", threshold:'SUCCESS'  ])])

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
            }
        }
    }
}
