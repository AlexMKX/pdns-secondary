FROM alpine:latest
RUN apk add ansible docker bind-tools py3-dnspython nftables docker-py iproute2 py3-jmespath py3-requests
RUN ansible-galaxy collection install community.docker

ENTRYPOINT ansible-playbook /onboot.yml
