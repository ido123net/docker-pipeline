node {
  checkout scm
  stage("Build") {
    image = docker.build("myimage")
  }
  stage("Test") {
    image.run()
  }
}
