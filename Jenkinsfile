
pipeline {
  agent any
  stages{
    stage("Maven Build"){
      when {
        branch "develop"
      }
      steps{
        echo "maven package"
      }
    }
    stage("Sonar Analysis"){
      when {
        branch "develop"
      }
      steps{
        echo "sonar analysis"
      }
    }
    stage("Dev Deploy"){
      when {
        branch "develop"
      }
      steps{
        echo "deploy to dev...."
      }
    }
    stage("Test Deploy"){
      when {
        branch "test"
      }
      steps{
        echo "deploy to test...."
      }
    }
     stage("Prod Deploy"){
      when {
        branch "main"
      }
      steps{
        echo "deploy to production...."
      }
    }
    
  }
}
