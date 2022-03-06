@Library('javahome-demo') _

pipeline{
    agent any
    stages{
        stage('Demo'){
            steps{
                welcome('Hari')
            }
        }
        stage("build-test") {
                    steps{
                        sh "mvn clean install"
                    }
                }
//                 stage("build-test") {
//                            steps {
//                                                sh "mvn -N help:effective-pom -Doutput=target/pom-effective.xml"
//
//                                                script {
//                                                    pom = readMavenPom(file: 'target/pom-effective.xml')
//                                                    projectArtifactId = pom.getArtifactId()
//                                                    projectGroupId = pom.getGroupId()
//                                                    projectVersion = pom.getVersion()
//                                                    projectName = pom.getName()
//                                                }
//
//                                                echo "Building ${projectArtifactId}:${projectVersion}"
//                                            }
//                                 }



    }
}
