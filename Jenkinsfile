@Library('javahome-demo') _

pipeline{
    agent any
    environment {
        //Use Pipeline Utility Steps plugin to read information from pom.xml into env variables
        IMAGE = readMavenPom().getArtifactId()
        VERSION = readMavenPom().getVersion()
        }

    stages{

        stage('Git branch'){
                    steps {
//                     sh "echo \{GIT_BRANCH}"
                        welcome('HAMID', "${GIT_BRANCH}", "${VERSION}")
                    }
        }
//         stage("build-test") {
//                     steps{
//                         sh "mvn clean install"
//                     }
//                 }

    }
}
