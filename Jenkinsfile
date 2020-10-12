pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'echo hello world'
                jfPipelines()
            }
        }
    }
}

jfPipelines(
  outputResources: """[
    {
      "name": "jenkins_job_results",
      "content": {
        "passing": 1234,
        "failing": 0
      }
    }
  ]"""
)
