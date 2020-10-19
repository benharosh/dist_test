pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'echo hello world'
                sleep 30s
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
