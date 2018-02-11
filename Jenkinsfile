node {
    // first repository<
    stage('Git Checkout'){
    git poll: true, url: 'https://github.com/spring-projects/spring-petclinic.git'
    }
    stage('Build'){
    env.JAVA_HOME = tool 'Java_8'
    bat 'mvn install'
    }    
}
