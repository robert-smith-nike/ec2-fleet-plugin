@Library('cop-pipeline') _

jarLibraryPipeline() {
    buildImage = 'maven:3.5-jdk-8'
    buildArtifacts = ['target/**/*']
    buildCmd = 'mvn clean install'
    testCmd = 'mvn test'
    publishCmd = 'mvn --settings $(pwd)/settings.xml -Dartifactory.user=$ARTIFACTORY_USER -Dartifactory.password=$ARTIFACTORY_PASSWORD deploy'
}
