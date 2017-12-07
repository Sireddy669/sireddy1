#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: '',
    projectUrlStr: 'https://github.com/Sireddy669/sireddy1.git/'],
    pipelineTriggers([
        upstreamProjects: 'https://github.com/Sireddy669/sireddy2.git'
        upstreamProjects: 'https://github.com/Sireddy669/sireddy3.git')])])

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
