pipeline {
  agent any
  stages {
    stage('JiraStatusChange') {
      steps {
        echo 'Bees Buzz!'
        jiraAddComment(idOrKey: 'JiraID', comment: 'adding comment from pipelint')
      }
    }

  }
  environment {
    JiraID = 'PRJ-3'
  }
}