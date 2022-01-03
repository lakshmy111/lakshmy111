pipeline {
  agent any
  stages {
    stage('JiraStatusChange') {
      steps {
        echo 'Bees Buzz!'
        jiraAddComment(idOrKey: 'PRJ-3', comment: 'adding comment from pipelint', site: 'JIRA')
      }
    }

  }
}