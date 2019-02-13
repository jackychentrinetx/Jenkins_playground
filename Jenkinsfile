pipeline {
  agent any
  stages {
    stage('connect_Snowflake') {
      steps {
        withCredentials( [usernamePassword( credentialsId: '1269ada7-a8ff-4a0b-a187-6749953013fe', 
                                      usernameVariable: 'USERNAME', 
                                      passwordVariable: 'PASSWORD')]) {
          sh 'snowsql -a nv34673.us-east-1 -u $USERNAME -m $PASSWORD -f test.snow'
        }
        echo 'Hi after pwd'
      }
    }
  }
}
