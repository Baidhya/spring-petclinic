node {
    // first repository<
    stage('Git Checkout'){
    git poll: true, url: 'https://github.com/spring-projects/spring-petclinic.git'
    }
    stage('Build'){
    bat '''set JAVA_HOME=\'C:\\Program Files\\Java\\jdk1.8.0_144\'
mvn install'''
    }    
}
