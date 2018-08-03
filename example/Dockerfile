FROM quay.io/shawn_hurley/ansible-operator

COPY roles /opt/ansible/roles
COPY playbooks/playbook.yaml /opt/ansible/playbook.yaml
COPY config.yaml /opt/ansible/config.yaml

RUN chmod -R g=u /opt/ansible
RUN adduser ansible-operator
USER ansible-operator
