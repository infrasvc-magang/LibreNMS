# LibreNMS

LibreNMS is an autodiscovering PHP/MySQL/SNMP based network monitoring which includes support for a wide range of network hardware and operating systems including Cisco, Linux, Juniper, Foundry, and many more.

## Installation

LibeNMS can be installed in 2 way, install with docker or install directly on server.

### Install Directly on Server

This [page](https://docs.librenms.org/Installation/Install-LibreNMS/) will show you how to do it, just follow the instruction and you will be fine.

### Install With Docker

Follow instruction bellow

1. Install docker: https://docs.docker.com/engine/install/
2. Download and unzip composer files:

   ```bash
   mkdir librenms
   cd librenms
   wget https://github.com/librenms/docker/archive/refs/heads/master.zip
   unzip master.zip
   cd docker-master/examples/compose
   ```
4. Set a new mysql password in .env and inspect docker-composer.yml (look .env and .yml file above for reference)
5. Bring up the docker containers
6. Open webui to finish configuration. http://localhost (use the correct ip or name instead of localhost)
   > note : add default port (8000) at the end of the web address since docker assign your ip using default port. (example http://localhost:8000)


