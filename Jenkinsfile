#!/usr/bin/env groovy
@Library('libcore@master') _

pipeline {
  agent {
    kubernetes {
      label 'maven-docker-pod'
      yamlFile 'mavenPod.yaml'
    }
  }
  stages {
    stage('Checkout') {
      steps {
        gitCheckout()
      }
    }
    stage ('App Build And Publish'){
      steps {
        appBuildPush()
      }
    }
    stage ('DOC Build And Push'){
      steps {
        dockerBuildPush()
      }
    }
  }
}