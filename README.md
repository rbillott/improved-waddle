# improved-waddle

## Setup
Pull the image.
```
docker pull ghcr.io/stormspectacular/testex02
```

Run the server.
```
docker run -it --rm -p 5000:5000 ghcr.io/stormspectacular/testex02
```

## Problem 
We have a python service providing a REST API to do some simple calculations.

A sample call for the REST API is as follows:
http://<ip>:35000/api/v1/calc_square?x=1


## Q1
The sever should accept connections on port 35000 as in the example shown above.
  
However currently that is not the case.

Fix the "docker run" command to listen on the correct port.

## Q2
Try the following queries below and observe the output of the service.

Describe what is wrong.

### API queries
http://<ip>:35000/api/v1/calc_square?x=1
http://<ip>:35000/api/v1/calc_square?x=2
http://<ip>:35000/api/v1/calc_square?x=3
http://<ip>:35000/api/v1/calc_square?x=25

## Q3 
Based on your observations in Q2, it's now time to fix the issues with the service!

Find a way to modify the python code and test your changes.


## Annex - Useful docker commands 
docker exec
https://docs.docker.com/engine/reference/commandline/exec/

docker logs
https://docs.docker.com/engine/reference/commandline/logs/

docker ps
https://docs.docker.com/engine/reference/commandline/ps/

docker run
https://docs.docker.com/engine/reference/run/


