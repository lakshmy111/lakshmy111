pipeline {
  agent any
  stages {
    stage('JiraStatusChange') {
      steps {
        echo 'Bees Buzz!'
        jiraAddComment(idOrKey: 'env.defectID', comment: 'adding comment from pipelint', site: 'JIRA')
      }
    }

  }
  environment {
    defectID = 'PRJ-2'
  }
}