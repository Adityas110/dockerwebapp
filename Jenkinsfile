node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        def customImage = docker.build("adityas1200/nodewebapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}