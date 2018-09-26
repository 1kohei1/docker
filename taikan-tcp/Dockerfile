FROM centos:7.0.1406
RUN yum swap -y -- remove fakesystemd -- install systemd systemd-libs
RUN yum -y install yum-plugin-ovl
RUN yum groupinstall -y 'Development Tools'
RUN yum install -y vim-enhanced.x86_64
COPY .gitconfig /root/
COPY .vimrc /root/
COPY auto-pairs.vim /root/.vim/plugin/
