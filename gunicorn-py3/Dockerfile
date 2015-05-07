FROM texastribune/gunicorn

# Remove python2 version of gunicorn
RUN /usr/bin/yes | pip uninstall -q gunicorn

# install python3 version of gunicorn and a nuch of useful packages commonly needed
RUN apt-get -yq update
RUN apt-get -yq install \
  git \
  python3-dev \
  python3-pip \
  libxml2-dev \
  libxslt-dev \
  libtiff5-dev \
  libjpeg8-dev \
  zlib1g-dev \
  libfreetype6-dev \
  liblcms2-dev \
  libwebp-dev \
  tcl8.6-dev \
  tk8.6-dev \
  python3-tk \
  libffi-dev \
  nodejs \
  npm

# Install bower
RUN npm install -g bower

RUN pip3 install gunicorn==19.1.1
