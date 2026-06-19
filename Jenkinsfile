pipeline{
  agent any
   stages
   {
    stage('Build'){
    steps{
    sh 'mvn clean compile'
    }
    }
    stage('Test'){
    steps{
    sh 'mvn test'
    }
    }
    stage('Package'){
    steps{
    sh 'mvn package'
    }
    }
    stage('Run'){
    steps{
    sh 'java -jar target/MavenApp-1.0-SNAPSHOT.jar'
    }
    }
    }
    }
