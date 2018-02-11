node {
    // first repository<
    env.JAVA_HOME = tool 'Java_8'
    stage('Git Checkout'){
    git poll: true, url: 'https://github.com/spring-projects/spring-petclinic.git'
    }
    stage('Build'){
    bat 'mvn install'
    }
    stage('SonarQube analysis') {
    // requires SonarQube Scanner 2.8+
    def scannerHome = tool 'Sonar_Cloud';
    withSonarQubeEnv('My SonarQube Server') {
      bat "${scannerHome}/bin/sonar-scanner"
    }  
    
}
