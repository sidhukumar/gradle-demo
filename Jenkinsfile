pipeline {
  agent any
  stages {
    stage('git') {
      steps {
        git(url: 'https://github.com/ghanigreen/gradle-demo.git', branch: 'master')
      }
    }
    stage('build') {
      steps {
        bat 'gradle build'
      }
    }
    stage('deploy') {
      steps {
        sh 'cp -r \'C:\\Program Files (x86)\\Jenkins\\workspace\\gradle-demo_master-7M6QKQFUTQY6COCIQH3W66FOS7GKC3IME4SDO4XR4DOPPQJZUJOA\\build\\libs\\jcg-gradle-war-example-1.0.war\' \'C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5\\webapps\''
      }
    }
  }
}