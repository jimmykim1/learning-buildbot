# please follow docker best practices
# https://docs.docker.com/engine/userguide/eng-image/dockerfile_best-practices/
# Dockerfile customizations for building buildbot's CI test suite.
#
# Provided here as a real life example on how to make a customized
# worker Dockerfile for your project

FROM        buildbot/buildbot-master:master
MAINTAINER  Buildbot Maintainers

# generate cache for the buildbot dependencies
RUN \
    pip install -U pip && \
    pip install networkx && \
    pip install gitpython
