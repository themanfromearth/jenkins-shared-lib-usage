node {
  stage('JIRA') {
    withEnv(['JIRA_SITE=JIRA']) {
      def testIssue = [fields: [ project: [key: 'TM'],
                                 summary: 'New JIRA Created from Jenkins.',
                                 description: 'New JIRA Created from Jenkins.',
                                 issuetype: [name: 'Task']]]

      response = jiraNewIssue issue: testIssue

      echo response.successful.toString()
      echo response.data.toString()
    }

  }
}