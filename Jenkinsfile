pipeline{
    agent any
    environment {
        PATH= "/opt/apache-maven-3.8.6/bin:$PATH"
    }
    stages{

    stage('Git clone'){
        steps{
            git credentialsId: '76b989ac-571a-41d3-b4bc-3f97a5e46e82', url: 'https://github.com/Kamasani-Sahadeva/hello-world.git'
        }

      }

      stage('Maven Build'){
        steps{
            sh 'mvn -version'
            sh 'mvn clean package'
        }

      }
    }


}
