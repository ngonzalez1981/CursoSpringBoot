node {
   def mvnHome
   stage('Preparation') { // for display purposes
      // Get some code from a GitHub repository
      // **       in the global configuration.     
      git 'https://github.com/lferna/CursoSpringBoot.git'
      mvnHome = tool 'Maven3'
   }
   stage('Build') {
         sh "'${mvnHome}/bin/mvn' -DskipTests clean package -X"       
   }
}
