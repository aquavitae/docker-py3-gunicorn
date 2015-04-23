FROM texastribune/gunicorn

# Remove python2 version of gunicorn
RUN /usr/bin/yes | pip uninstall -q gunicorn

# install python3 version of gunicorn
RUN apt-get -yq update
RUN apt-get -yq install \
  git \
  python3-dev \
  python3-pip

RUN pip3 install gunicorn==19.1.1
