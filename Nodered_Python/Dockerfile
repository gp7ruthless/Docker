# docker build . -t nodered_gg
# docker run -i -p 1880:1880 -v ./node-red:/root/.node-red --name nodered_GG nodered_gg
FROM python:3.9.13
USER root
RUN cat /etc/os-release
RUN apt update
RUN apt install cmake -y
RUN pip install awsiotsdk
RUN apt install nodejs npm -y
RUN npm install -g --unsafe-perm node-red
COPY ./python_scripts/. /python_scripts/.
CMD [ "node-red" ]
