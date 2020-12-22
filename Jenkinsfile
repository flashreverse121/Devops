node {

    checkout scm

    docker.withRegistry('https://hub.docker.com/repository/docker/kohopay/', 'dockerHub') {

        def customImage = docker.build("docker-testing/dockerwebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
