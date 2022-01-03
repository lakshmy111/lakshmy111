pipeline {
  agent any
  stages {
    stage('JiraStatusChange') {
      steps {
        echo 'Bees Buzz!'
        jiraAddComment(idOrKey: 'JIRA_ISSUE_KEY', comment: 'adding comment from pipelint', site: 'JIRA')
      }
    }

  }
}