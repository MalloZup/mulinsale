FROM opensuse:42.2
MAINTAINER Michele Bologna <michele.bologna@gmail.com>

RUN zypper --non-interactive in -y salt-minion && \
	zypper clean
COPY minion.conf /etc/salt/minion
