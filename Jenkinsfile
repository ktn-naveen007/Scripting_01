node('master'){
echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
stage('initialize'){
checkout scm
}
stage('compile'){
 bat '''
mvn compile
'''
}
stage('unittest'){
bat '''
mvn test
'''
}

}