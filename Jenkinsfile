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
        sh 'cp -r \'C:\\Program Files (x86)\\Jenkins\\workspace\\gradle-demo\\build\\libs\\jcg-gradle-war-example-1.0.war\' \'C:\\Program Files\\Apache Software Foundation\\Tomcat 8.5\\webapps\''
      }
    }
  }
}