node {
    // first repository<
    stage('Git Checkout'){
    git poll: true, url: 'https://github.com/spring-projects/spring-petclinic.git'
    }
    stage('Build'){
    bat 'mvn install'
    }    
}
