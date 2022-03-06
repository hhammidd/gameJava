@Library('javahome-demo') _

pipeline{
    agent any
    stages{
        stage('Demo'){
            steps{
                welcome('Hari')
            }
        }
        stage('Git branch'){
                    steps {

                        welcome($GIT_BRANCH)
                    }
        }
//         stage("build-test") {
//                     steps{
//                         sh "mvn clean install"
//                     }
//                 }

    }
}
