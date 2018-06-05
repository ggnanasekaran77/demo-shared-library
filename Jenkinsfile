#!/usr/bin/groovy

pipeline {
    agent none
    stage ('Example') {
        steps {
             script {
                 library 'my-shared-library@master'
                 log.info 'Starting'
                 log.warning 'Nothing to do!'
             }
        }
    }
}