node {
    // first repository<
    stage('Git Checkout'){
    checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [[$class: 'RelativeTargetDirectory', relativeTargetDir: 'subdirectory1']], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/spring-projects/spring-petclinic.git']]])
    }
}
