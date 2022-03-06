@Library('javahome-demo') _

pipeline{
    agent any
    stages{

        stage('Git branch'){
                    steps {
//                     sh "echo \{GIT_BRANCH}"
                        welcome('HAMID', "${GIT_BRANCH}", "${BUILD_NUMBER}")
                    }
        }
//         stage("build-test") {
//                     steps{
//                         sh "mvn clean install"
//                     }
//                 }

    }
}
