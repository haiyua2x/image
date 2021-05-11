 pipeline {
    agent any

    stages {
       stage('build') {
          steps {
             echo 'Notify GitLab Build'
             updateGitlabCommitStatus name: 'build', state: 'pending'
             updateGitlabCommitStatus name: 'build', state: 'success'
             echo 'build done'
          }
       }
        stage('test1') {
          steps {
             echo 'Notify GitLab Test'
             updateGitlabCommitStatus name: 'test1', state: 'pending'
             updateGitlabCommitStatus name: 'test1', state: 'success'
          }
       }
       stage('test2') {
          steps {
             echo 'Notify GitLab Test'
             updateGitlabCommitStatus name: 'test2', state: 'pending'
             updateGitlabCommitStatus name: 'test2', state: 'success'
          }
       }
    }
 }
