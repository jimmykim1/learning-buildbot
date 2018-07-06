FROM        buildbot/buildbot-worker:master
MAINTAINER  Buildbot Maintainers

# generate cache for the buildbot dependencies
RUN \
    mkdir -p /tmp/bb && \
    curl -sL https://github.com/buildbot/buildbot/archive/master.tar.gz | \
    tar  --strip-components=1 -C /tmp/bb -xz && \
    virtualenv /tmp/bb/sandbox && \
    . /tmp/bb/sandbox/bin/activate && \
    pip install -U pip && \
    pip install networkx && \
    pip install gitpython && \
    rm -rf /tmp/bb
