FROM  alpine:latest 
RUN   apk update
RUN   apk add python3
RUN   apk add py3-pip
RUN   apk add sshpass
RUN   apk add py3-paramiko
RUN   apk add ansible
RUN   ansible-galaxy collection install arista.eos
RUN   ansible-galaxy collection install ansible.netcommon
WORKDIR /ansible
CMD [ "ansible-playbook", "--version" ]
#:wCMD ["ansible-playbook","-vvv",  "-i", "inventory", "playbook.yaml"]
#CMD ["ls -l /tmp"]
#CMD ["ansible-playbook", "--version"]
