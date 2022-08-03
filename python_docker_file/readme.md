Instructions : 

Folder Structure :

<Folder_Name>
....app/
        ....<Python Application with driver file named as 'main.py'>
....Dockerfile
....requirements.txt


Commands :
  docker build -t <image_name> .
  docker run -i -t <image_name>                   # -i to run input terminal inside the container
