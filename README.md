# Ansible Role Sonar

* Deploys sonar using [Docker Compose](https://git.spatz.wtf/infrastruktur/sonarqube-docker)
* Systemd service for starting and restarting
* Uses submodule instead of just cloning docker-compose repo because the templates (`files/sonarqube-docker/init-letsencrypt.template`) have to be executed before deployment to insert the proper hostname.