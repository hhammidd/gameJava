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

        stage('version'){
                             IMAGE = readMavenPom().getArtifactId()
                                VERSION = readMavenPom().getVersion()
                                echo "IMAGE: ${IMAGE}"
                                echo "VERSION: ${VERSION}"
                        }

    }
}
