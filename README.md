# skaffold-node-js-getting-started
Boilerplate to get started with local development for Kubernetes using Skaffold, Minikube and a Node.js HTTP server



## Requirements
Install the necessary technologies:
- [Install Node.js](https://nodejs.org/en/download/current/)
- [Install Docker](https://docs.docker.com/get-started/)
- [Install Skaffold](https://skaffold.dev/docs/install/)
- [Install kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)
- [Install minikube](https://minikube.sigs.k8s.io/docs/start/)



## Development

Make sure that your minikube cluster is running with: `minikube start`

Run `skaffold dev` to trigger the build and deploy process via skaffold.

When your server is running use `minikube service skaf-app-svc` to expose the the k8s service defined in the `k8s-service.yaml` to your local machine, so you can access it via the IP + Port. 

The `minikube service $SERVICE` should also open a new browser tab where you can see a request to the root level of your running server.

