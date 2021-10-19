running:
- ./paho-web-docker
- sudo docker build -t web-tag . 
- sudo docker run --name web-app -d -p 8080:80 web-tag 