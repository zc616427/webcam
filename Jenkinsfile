#!/usr/bin/env groovy
def remote = [:]
remote.allowAnyHosts = true

version = "1.0.0"

pipeline {
    agent any

    stages {
		stage('Maven Build') {
            steps {
                bat "mvn -U -am clean package -DskipTests"
            }
        }
    }
}
