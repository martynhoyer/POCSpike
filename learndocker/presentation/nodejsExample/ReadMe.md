
### Check if Docker is installed

`docker --version`

### Build

`docker build -t talk/nodejsexample:1.0 .`

### Run your docker image

`docker run -d -p 9080:9080 talk/nodejsexample:1.0`

### To test

Locally: `curl http://127.0.0.1:9080/`

Lan:

* Get your IP: `ifconfig | grep "inet " | grep -v 127.0.0.1`
* curl `http://<YourIP>:9080`