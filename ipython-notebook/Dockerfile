FROM dockerfile/ubuntu
MAINTAINER Sam Wing <sampwing@gmail.com>

RUN \
    apt-get update && \
    apt-get install -y python-numpy python-scipy python-matplotlib ipython ipython-notebook python-pandas python-sympy python-nose

RUN mkdir -p /data/notebook

EXPOSE 8888

CMD ["ipython", "notebook",  "--ip=*", "--notebook-dir=/data/notebook", "--pylab=inline", "--no-browser"]
