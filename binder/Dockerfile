FROM gesiscss/binder-r2d-g5b5b759-serhatcevikel-2dad454-4c1efa:d1c206768994994f8fd8f496464c31e31a644cf6
LABEL maintainer="serhatcevikel@yahoo.com"

USER ${NB_USER}

RUN \
    rm -r ${HOME}/*;

# Make sure the contents of our repo are in ${HOME}
COPY --chown=jovyan:jovyan . ${HOME}

RUN \
    rm -r ${HOME}/binder;

# Specify the default command to run
WORKDIR ${HOME}
