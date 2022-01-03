pipeline {
  agent any
  stages {
    stage('JiraStatusChange') {
      steps {
        echo 'Bees Buzz!'
        echo "Issue key is ${defectID}"
        echo "The build number is ${env.BUILD_NUMBER}"
        jiraAddComment(idOrKey: "${defectID}", comment: 'adding comment from pipelint', site: 'JIRA')
      }
    }

  }
  environment {
    defectID = 'PRJ-2'
  }
}