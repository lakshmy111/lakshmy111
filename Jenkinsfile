pipeline {
  agent any
  stages {
    stage('JiraStatusChange') {
      steps {
        echo 'Bees Buzz!'
        jiraAddComment(idOrKey: '$defectid', comment: 'adding comment from pipelint', site: 'JIRA')
        echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
      }
    }

  }
}