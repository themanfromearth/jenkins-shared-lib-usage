node {
  stage('JIRA') {
    withEnv(['JIRA_SITE=JIRA']) {
      # Look at IssueInput class for more information.
      def testIssue = [fields: [ // id or key must present for project.
                                 project: [key: 'TM'],
                                 summary: 'New JIRA Created from Jenkins.',
                                 description: 'New JIRA Created from Jenkins.',
                                 customfield_1000: 'customValue',
                                 // id or name must present for issueType.
                                 issuetype: [id: '3']]]

      response = jiraNewIssue issue: testIssue

      echo response.successful.toString()
      echo response.data.toString()
    }

  }
}