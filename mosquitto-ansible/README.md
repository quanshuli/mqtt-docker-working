running commands:

./mosquitto-docker
- sudo docker run -it -p 1883:1883 -p 9001:9001 -v mosquitto.conf:/mosquitto/config/mosquitto.conf eclipse-mosquitto 

or 
./
- ansible-playbook mosquitto_ansible.yml -K (without docker-compose.yml)

or with docker compose
- ansible-playbook mosquitto-container.yml


Requirements to run the script:
- Docker Engine
- Docker API >= 1.20
- Docker SDK for Python: Please note that the docker-py Python module has been superseded by docker (see here for details). For Python 2.6, docker-py must be used. Otherwise, it is recommended to install the docker Python module. Note that both modules should not be installed at the same time. Also note that when both modules are installed and one of them is uninstalled, the other might no longer function and a reinstall of it is required.
- Docker SDK for Python >= 1.8.0 (use docker-py for Python 2.6)
- PyYAML >= 3.11
- docker-compose >= 1.7.0