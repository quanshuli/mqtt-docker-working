running:
./paho-web-docker
- using docker 
- sudo docker build -t web-tag . 
- sudo docker run --name web-app -d -p 8080:80 web-tag 

or 
./ 
- using ansible
- ansible-playbook paho-web-ansible.yml -K

Requirements to run the script:
- Docker Engine
- Docker API >= 1.20
- Docker SDK for Python: Please note that the docker-py Python module has been superseded by docker (see here for details). For Python 2.6, docker-py must be used. Otherwise, it is recommended to install the docker Python module. Note that both modules should not be installed at the same time. Also note that when both modules are installed and one of them is uninstalled, the other might no longer function and a reinstall of it is required.
- Docker SDK for Python >= 1.8.0 (use docker-py for Python 2.6)
- PyYAML >= 3.11
- docker-compose >= 1.7.0