# Project Spark Elasticsearch

## Students
- Marwan MASHRA 
- Abdurrahman SHAHID 
- Romain MAGNET

## Files
* <b>stream.ipynb</b> : the server that streams tweets from the Twitter API.
* <b>process.ipynb</b> : Spark & Elasticsearch

## How to run
1) Start by launching the server from <b>stream.ipynb</b>. The port by default is <b>4040</b> but you can change it. Also you can change the Bearer_token if you want to. Run it and make sure you're server is listening to the port you choose (it shows a message).
2) Launch a server Elasticsearch (in a docker container or not). We assume that you'll use the port 9200, but you can choose another one.
3) Put the file <b>process.ipynb</b> in an environment where spark is installed, we used a docker container, but you can use what you want. Change the ports in the top according to the ports you chose previously (STREAM_PORT, ELASTIC_PORT). No need to change them if you used the default ones.
4) In the same place, change the host to <b>localhost</b> if you're not running the code in a docker container. if you're, keep it at <b>host.docker.internal</b>
5) You can now run the code of <b>process.ipynb</b>.
