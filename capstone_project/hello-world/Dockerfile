FROM node:16
#Update APT repository & Install OpenSSH
RUN apt-get update \
    && apt-get install -y openssh-server \
    && mkdir -p /var/run/sshd \
    && apt-get install sudo
#Set Root password
RUN useradd -rm -d /home/ansible_controller -s /bin/bash -g root -G sudo -u 1001 ansible_controller
RUN echo ansible_controller:12345 | chpasswd
RUN echo "ansible_controller ALL=(ALL:ALL) NOPASSWD: ALL" |  EDITOR="tee -a"  visudo
#RUN service ssh start
RUN /etc/init.d/ssh start
EXPOSE 22

# App Folder
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app
# Install app dependencies
COPY . /usr/src/app/
RUN npm install
# Bundle app source
EXPOSE 3000
CMD npm start


