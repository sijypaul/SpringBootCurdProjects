pipeline
{
    agent any
    stages 
    {
        stage('git repo & clean') 
        {
            steps
            {
              // bat "rmdir  /s /q assesmentfile"
               bat "git clone https://github.com/sijypaul/SpringBootCurdProjects.git"
                bat "mvn clean -f SpringBootCurdProjects"
            }
        }
       
        stage('package')
        {
            steps 
            {
                bat "mvn package -f SpringBootCurdProjects"
            }
        }
    }
}
