FROM        buildbot/buildbot-worker:master
MAINTAINER  Buildbot Maintainers

USER root

# generate cache for the buildbot dependencies
RUN \
    pip install -U pip && \
    pip install networkx && \
    pip install gitpython

USER buildbot
