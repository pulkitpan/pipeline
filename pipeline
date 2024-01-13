pipeline
{
    agent any
    stages
    {
        stage('fetch')
        {
            steps{
            git branch: 'main', url: 'https://github.com/pulkitpan/maven.git'
            }
        }
        
        stage('build')
        {
            steps{
            build 'maven_job'
            }
        }
        stage('Test')
        {
            steps{
            echo "Testing..Phase"
            }
        }
        stage('Deploy')
        {
            steps{
            echo 'Deploying..Phase'
            }
        }
    }
}
