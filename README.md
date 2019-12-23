Codenvy Docker
This file is used to generate the image/environment on which your Codenvy projects will be set up.

Building the Image
Running Commands
Pushing to Docker Hub
Running with Codenvy
This docker image installs and sets up the following:

Ruby
Rails
Postgres
Node.js
Codenvy necessities
Building the Image
To build the image:

docker build . -t trilogyed/codenvy
Running Commands
To run commands interactively in a new container using the image:

docker run -i -t trilogyed/codenvy /bin/bash
Pushing to Docker Hub
Submit a PR with changes to https://github.com/coding-boot-camp/codenvy-docker

Currently this image is publicly available on docker hub here: https://hub.docker.com/r/trilogyed/codenvy/ .

Running with Codenvy
To run this on Codenvy, simply create a new stack with the following recipe:

FROM trilogyed/codenvy
Then, when creating a new workspace, choose the stack with the name used in the creation above.
