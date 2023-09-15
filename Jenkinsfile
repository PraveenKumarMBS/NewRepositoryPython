pipeline
{
    agent any
    parameters
    {
        choice(choices: 'dev\ntest\nstage\nwhat-if\nprod\nbatch, description: 'select the target environment.', name: 'Environment')4
        gitparameter(defaultValue: 'origin/main', description: 'Branch/tag to build and deploy', name: 'BRANCH_TAG', type: 'PT_BRANCH_TAG')
    }
    stages
    {
        stage("build")
        {
            steps
            {
                echo 'building the application'
            }
        }
        stage("test")
        {
            steps
            {
                echo 'testing the application'
            }
        }
        stage("deploy")
        {
            steps
            {
                echo 'deploying the application'
            }
        }
    }
}
