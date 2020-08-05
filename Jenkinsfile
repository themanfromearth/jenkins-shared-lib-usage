@Library('jenkins-shared') _

node {
  stage('JIRA') {

    def testIssue = [fields: [
                               project: [id: 'TM'],
                               summary: 'New JIRA Created from Jenkins.',
                               description: 'New JIRA Created from Jenkins.',
                               issuetype: [id: '3']]]

    response = jiraNewIssue issue: testIssue

    echo response.successful.toString()
    echo response.data.toString()

    apiPipeline
  }
}

