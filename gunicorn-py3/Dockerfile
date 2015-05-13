FROM texastribune/gunicorn

# Remove python2 version of gunicorn
RUN /usr/bin/yes | pip uninstall -q gunicorn

RUN pip3 install gunicorn==19.1.1

