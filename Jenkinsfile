#!/usr/bin/env groovy

pipeline {
    agent any

    stages {
        stage('Building Docker Image') {
            steps {
             	script {
                 		@library ('my-shared-library@master')
                		log.info 'Starting'
                 		log.warning 'Nothing to do!'
                 		build 'Hello World'

            	 }
            }
        }
    }
}