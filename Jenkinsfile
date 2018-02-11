node {
    // first repository<
    env.JAVA_HOME = tool 'Java_8'
    stage('Git Checkout'){
    git poll: true, url: 'https://github.com/spring-projects/spring-petclinic.git'
    }
    stage('Build'){
    bat 'mvn install'
    }
    stage('Sonar analysis'){
     bat 'mvn sonar:sonar -Dsonar.organization=baidhya-github -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=8a95571235aae6b422332de51ecd79317afadaef'
    }
    
}
