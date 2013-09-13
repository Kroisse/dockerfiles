FROM	kroisse/ruby19

RUN	gem install gollum redcarpet
RUN	apt-get install -y python2.7 curl git-core
RUN	curl https://bitbucket.org/pypa/setuptools/raw/bootstrap/ez_setup.py | python
RUN	easy_install docutils
RUN	mkdir -p /var/local/gollum/wiki && git init /var/local/gollum/wiki

EXPOSE	4567
CMD	["gollum", "/var/local/gollum/wiki"]
