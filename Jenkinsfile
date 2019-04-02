#!/usr/bin/env groovy
@Library('libcore@master') _
pipeline {
    agent any

    stages {
        stage('gitCheckout') {
            steps {
             	script {
             	gitCheckout()
            	 }
            }
        }
        stage ('App Build And Publish'){
            steps {
                script {
                appBuildPush()
                }
            }
        }
        stage ('DOC Build And Push'){
            steps {
                script {
                    dockerBuildPush()
                }
            }
        }
    }
}