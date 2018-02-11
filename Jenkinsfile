node {
    // first repository<
    stage('Git Checkout'){
    git url: 'https://github.com/spring-projects/spring-petclinic.git'
    }
    stage('Build'){
    sh 'mvn install'
    }    
}
