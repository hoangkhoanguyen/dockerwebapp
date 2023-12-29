node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub-hoangkhoanguyen') {

        def customImage = docker.build("hoangkhoanguyen/karaoke-clone:test-jenkins")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
