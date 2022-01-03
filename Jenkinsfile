pipeline {
  agent any
  stages {
    stage('JiraStatusChange') {
      steps {
        echo 'Bees Buzz!'
        sh '''echo "I am ${defectID}" 
sh \'./jenkins/build.sh\''''
        jiraAddComment(idOrKey: 'env.defectID', comment: 'adding comment from pipelint', site: 'JIRA')
      }
    }

  }
  environment {
    defectID = 'PRJ-2'
  }
}