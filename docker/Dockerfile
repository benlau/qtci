FROM ubuntu:18.04
VOLUME ["/host/qtci", "/host/download"]

# USERID should be same as the current user.
ARG USERID
ARG USERNAME=ci

ENV DISPLAY=":0"

RUN useradd --create-home --no-user-group -u $USERID $USERNAME -s /bin/bash && adduser $USERNAME sudo

RUN apt-get update && \
	apt-get install -y --no-install-recommends ansible sudo && \
	rm -rf /var/lib/apt/lists/* && \
    apt-get clean 

ADD ansible.yml /host/ansible.yml

RUN ansible-playbook /host/ansible.yml && \
	rm -rf /var/lib/apt/lists/* && \
    apt-get clean 

USER $USERNAME

WORKDIR /home/$USERNAME

CMD ["bash"]

