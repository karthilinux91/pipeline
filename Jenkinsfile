pipeline {
  agent any
  stages {
    stage('SQA-Blink-01') {
      steps {
        build 'SQA-Blink-01'
      }
    }
    stage('SQA-InjectError-02') {
      steps {
        build(job: 'SQA-InjectError-02', propagate: true)
      }
    }
  }
}