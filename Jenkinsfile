node {

  def app
     stage('Clone') {
        checkout scm
     }

     stage('Build image') {
        app = docker.build("krusser/nginx")
     }

    stage('Test image') {
        docker.image('krusser/nginx').withRun('-p 80:80') { c ->
        sh 'docker ps'
     }
  }
}
