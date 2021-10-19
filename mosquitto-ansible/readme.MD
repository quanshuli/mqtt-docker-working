running commands:

./mosquitto-docker
sudo docker run -it -p 1883:1883 -p 9001:9001 -v mosquitto.conf:/mosquitto/config/mosquitto.conf eclipse-mosquitto 

or
./
ansible-playbook mosquitto_container.yml -K 