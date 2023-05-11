pipeline {
  agent {
  label 'ubuntu'
}

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                sh "pwd"
                sh "kubectl version"
                sh "helm version"
                sh "cd drupal; helm upgrade my-release helm-drupal --values ./helm-drupal/values.yaml"
                
            }
        }
    }
}
