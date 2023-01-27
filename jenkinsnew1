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
    stage('continous Deployment_master')
    {
        cicd.newDeploy("Scriptedwithsharedlibrary","172.31.30.227","testapp")
    }
    stage('continous Testing_master')
    {
     cicd.newGit("https://github.com/intelliqittrainings/FunctionalTesting.git")
     cicd.runselenium("Scriptedwithsharedlibrary")
    }
    stage('continous Delivery_master')
    {
      cicd.newDeploy("Scriptedwithsharedlibrary","172.31.31.86","prodapp") 
    }
}
