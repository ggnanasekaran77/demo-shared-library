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

/*
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (App Build And Publish)
[Pipeline] script
[Pipeline] {
[Pipeline] libraryResource
[Pipeline] echo
Hello World Hello Gradle Build
[Pipeline] echo
gradlepodtemplate: testing
testng
tastk

[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] stage
[Pipeline] { (DOC Build And Push)
[Pipeline] script
[Pipeline] {
[Pipeline] echo
Hello World dockerBuildPush
[Pipeline] }
[Pipeline] // script
[Pipeline] }
[Pipeline] // stage
[Pipeline] }
[Pipeline] // withEnv
[Pipeline] }
[Pipeline] // node
[Pipeline] End of Pipeline
Finished: SUCCESS
*/