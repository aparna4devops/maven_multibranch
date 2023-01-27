@Library('newlibrary')_
node('built-in')
{
    stage('continous Download_loans')
    {
      cicd.newGit("https://github.com/aparna4devops/mymaven16.git")
    }
    stage('continous build_loans')
    {
      cicd.newmaven()
    }
}
    
