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
    }
}