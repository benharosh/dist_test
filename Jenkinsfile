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
      "name": "jenkins_job_master",
      "content": {
        "passing": 1234,
        "failing": 0
      }
    }
  ]"""
)
