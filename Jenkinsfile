pipeline{
    agent any
    tools{
        // Install the maven version configured as "M3" and add it to the path.
        maven "maven3"
        }
stages{
    stage("get scm"){
        steps{
         git credentialsId: 'github_crediantials', url: 'https://github.com/Sowparn/spring3-mvc-maven-xml-hello-world.git'
        }
    }  
    stage("build"){
        steps{
            sh "mvn package"
          }              
        }
     }    
}
