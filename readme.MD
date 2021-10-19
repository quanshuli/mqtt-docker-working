./paho-web
- this directory is the web sever container, in this container the web app is receiving the signals.

./paho-ansible
- this directory is the signal sending container, in which paho-mqtt python package is used to send the signals.

./mosquitto-ansible
- this directory is the mosquitto container to transfer messages.