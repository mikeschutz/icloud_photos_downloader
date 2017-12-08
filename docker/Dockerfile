FROM ubuntu:latest

RUN apt-get update && \
    apt-get -y install python python-pip git ca-certificates && \
    git clone https://github.com/mikeschutz/icloud_photos_downloader.git && \
    pip install -r icloud_photos_downloader/requirements.txt && \
    useradd -u 1000 -b /home/user user

USER user

WORKDIR /icloud_photos_downloader
