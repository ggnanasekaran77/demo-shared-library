#!/usr/bin/groovy

@Library('my-shared-library')

pipeline {
    agent none
    stage ('Example') {
        steps {
             script {
                 log.info 'Starting'
                 log.warning 'Nothing to do!'
             }
        }
    }
}