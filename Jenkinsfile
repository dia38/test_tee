pipeline
{
    agent none
    
    stages
    {
        stage('Build 1')
        {
            agent {
                label 'wct_build_windows_nju_laptop'
            }
            steps
            {
                tee('Log1.txt')
                {
                    sh 'ls -la'
                    echo "Build 1"
                    sleep 5
                    echo "Build 2"
                }
            }
        }
        stage('Build 2')
        {
            agent {
                label 'wct_build_windows_nju_laptop'
            }
            steps
            {
                tee('Log2.txt')
                {
                    sh 'ls -la'
                    echo "Build 3"
                    sleep 5
                    echo "Build 4"
                }
            }
        }
    }
}
