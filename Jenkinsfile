pipeline {
  agent any
  stages {
    stage('JiraStatusChange') {
      steps {
        echo 'Bees Buzz!'
        echo "Issue key is ${env.defectID}"
        echo "The build number is ${env.BUILD_NUMBER}"
        echo "The env jira key is ${env.defectID}"
        bat './jenkins/build.bat'
        jiraAddComment(idOrKey: "${defectID}", comment: 'adding comment from pipelint', site: 'JIRA')
      }
    }

  }
}