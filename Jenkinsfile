#!/usr/bin/groovy

pipeline {
    agent none
    stage ('Example') {
        steps {
             script {
                 @Library('my-shared-library')
                 log.info 'Starting'
                 log.warning 'Nothing to do!'
             }
        }
    }
}