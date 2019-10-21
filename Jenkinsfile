node {

    checkout scm

    docker.withRegistry('https://hub.docker.com', 'dockerHub') {

        def customImage = docker.build("ahamedn/hellowhale")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
