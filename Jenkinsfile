pipeline {
    agent any 
        stages{
            stage('Run quality checks'){
                when {
                    branch 'main' 
                }
              steps {
                    sh '/var/lib/jenkins/tools/hudson.plugins.sonar.SonarRunnerInstallation/sonar/bin/sonar-scanner \
  -Dsonar.projectKey=hirsonu \
  -Dsonar.sources=. \
  -Dsonar.host.url=http://13.232.74.162:9000 \
  -Dsonar.login=sqp_e54473f39e2be38a9da075440179d8e8d578156d'
            }
        }
        
    }
}
