pipeline
{
    agent any
    // environment {
    //     def mavenHome = tool 'maven'
    // }
    stages
    {
        stage("build-code")
        {
            steps
            {
                sh "mvn install "
                sh "ls -lrt target/"
            }
        }
        stage("Run Unit Tests"){
            steps {
               sh "mvn test"
            }
        }
    }
}
