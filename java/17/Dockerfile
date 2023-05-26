FROM ghcr.io/pterodactyl/yolks:java_17

USER root

RUN apt update && apt install wget
RUN wget -q -O /tmp/tinyspline.deb https://objects.githubusercontent.com/github-production-release-asset-2e65be/24473646/c6c7b31d-37d2-4753-aaad-559b45d00107?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIWNJYAX4CSVEH53A%2F20230526%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20230526T194110Z&X-Amz-Expires=300&X-Amz-Signature=1899967360e345cfd6d8c6c8e0d777ee1a58bafe60404829761562490a87e453&X-Amz-SignedHeaders=host&actor_id=63400965&key_id=0&repo_id=24473646&response-content-disposition=attachment%3B%20filename%3Dtinyspline-0.6.0-Linux.deb&response-content-type=application%2Foctet-stream \
    && dpkg -i /tmp/tinyspline.deb \
    && rm /tmp/tinyspline.deb

USER container