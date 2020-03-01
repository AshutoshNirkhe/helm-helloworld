# Helm chart for Hello World!
Helm chart for sample Hello World node.js app



### Hello World node.js app
- 'helloworld-nodejs-app' contains the 'server.js' code that prints out Hello World. It also prints the URI details. Can be tested standlone with 'node server.js' assuming node.js is installed.
- 'helloworld-nodejs-app' contains 'Dockerfile' that dockerizes this little node.js app. Docker image for the same can be found on https://hub.docker.com/repository/docker/a5hut0sh/helloworld


### install helm chart 
- 'helm-chart/helloworld' contains all the template yamls for deploying the Hello World node.js app in kubernetes.
- Modify values.yaml to suit your needs.
- Install the chart 
$ helm install --name helloworld . --namespace hello


### Sample output

$ curl http://localhost/hello

Received request from URL : /hello

Hello World!

$ curl http://localhost/testurl

Received request from URL : /testurl

Hello World!
