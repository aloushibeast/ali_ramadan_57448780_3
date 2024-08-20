FROM "image": "mcr.microsoft.com/devcontainers/universal:2-linux"
# Install the xz-utils package
RUN apt-get update && \
apt-get install -y xz-utils mongodb && \
pip install django

RUN mkdir -p /data/db

EXPOSE 8000 27017

CMD ["mongod", "--bind_ip_all"]