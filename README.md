# Multi-node Docker Lab Builder

A little script and a few docker compose files for building multi node Graylog setups in Docker.

Pre-Requisities: 
- Docker 
- Docker Compose v3
- Mac or Linux OS.

How to use: 
- Save and unzip the folder somewhere that the current user has access to read/modify/execute.
- Navigate inside the folder and run the "launch-cluster.sh" script from the terminal. Note: on Mac you may need to chmod 775 the "launch-cluster.sh" file.
- Follow the instructions within the terminal window.
- Once your lab has been spun up, you can connect to it on http://127.0.0.1:80/
- Default logon credentials to the UI are admin/admin.

Good to know:
- All mongoDB and Elastic/Opensearch data is persistently stored in ./storage
- Graylog storage (Journal etc) is persistant but not accessible.
- There is a script in ./scripts called "mongo-cluster-comand.sh". You should run this to make the Mongo nodes form a cluster after bringing the containers up again after a shutdown.
