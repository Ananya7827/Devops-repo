pipeline { 
   agent any 
   stages {
     stage('Clone Repo') { 
      steps { git branch: 'main', url: 'git@github.com:Ananya7827/Devops-repo.git' } } 
      stage('Build Docker Image') { 
      steps { sh 'docker build -t brand-store .' } }
     stage('Run Container') { 
     steps { sh 'docker run -d -p 8080:80 brand-store'
      }
   }
  }
 }
