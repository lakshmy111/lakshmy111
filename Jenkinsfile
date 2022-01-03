pipeline {
  agent any
  stages {
    stage('JiraStatusChange') {
      steps {
        echo 'Bees Buzz!'
        jiraAddComment(idOrKey: 'params.defectid', comment: 'adding comment from pipelint', site: 'JIRA')
      }
    }

  }
}