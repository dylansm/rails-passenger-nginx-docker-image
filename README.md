docker-base
===========

- nginx
- passenger 4.0.29
- ruby 2.1.0

For more versions see Dockerfile.


Getting Started
---------------

Get the image via index.docker.io

        $ docker pull networld/docker-base

        or build from source

        $ IMAGE_NAME=networld/docker-base
        $ docker build -rm -t ${IMAGE_NAME} .

Start a container with:

        $ docker run -rm -p 127.0.0.1:8181:80 -d -v /path/to/ruby_on_rails_app:/webapp ${IMAGE_NAME}
        $ curl http://127.0.0.1:8181 # Test with curl or even better your favorite browser


For more information see https://index.docker.io/u/networld/docker-base/ and
the source code under https://github.com/networld-to/docker-base

