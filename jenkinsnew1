@Library('newlibrary')_
node('built-in')
{
    stage('continous Download_master')
    {
      cicd.newGit("https://github.com/aparna4devops/mymaven16.git")
    }
    stage('continous build_master')
    {
      cicd.newmaven()
    }
    
