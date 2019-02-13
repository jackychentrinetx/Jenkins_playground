pipeline {
  agent any
  stages {
    stage('connect_Snowflake') {
      steps {
        sh 'snowsql -a nv34673.us-east-1 -u jchen -M -f test.snow'
        echo 'Hi after pwd'
      }
    }
  }
}