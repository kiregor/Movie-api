pipeline{
        agent any
        stages{
                stage('---clean---'){
                        steps{
                                sh "mvn clean"
                        }
                }
                stage('--test--'){
                        steps{
                                sh "mvn test"
                        }
                }
                stage('--package--'){
                        steps{
                                sh "mvn package"
                        }
                }
                stage('--deployment--'){
                        steps{
                                sh "cp /var/lib/jenkins/workspace/Test/target/movieapp.war /home/daniellake89/wildfly-10.1.0.Final/standalone/deployments
                        }
                }
        }
}
