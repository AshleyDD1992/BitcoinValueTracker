# BitcoinValueTracker
### An Elastic stack set up to track the value of bitcoin using the coindesk api
Logstash to ingest, Elasticsearch to store, Kibana to visualiza and Nginx to secure the data.

## How to
These instructions assume that docker and docker-compose are already installed, if that is not the case please do so first.
1. Clone the repo `git clone git@github.com:AshleyDD1992/BitcoinValueTracker.git￼`
2. Install httpd_tools `apt-get install httpd-tools`
3. Move into nginx/etc folder `cd ~/BitcoinValueTracker/nginx/etc`
4. Create username and password for Kibana `htpasswd -c .htpasswd.user <username>`
5. Launch containers `docker-compose up -d`
6. Hit kibana endpoint at `localhost/kibana`
