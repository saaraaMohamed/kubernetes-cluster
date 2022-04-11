# kubernetes-cluster
kubernetes cluster.
1- Create a deployment of 2 replicas using image of  linuxacademycontent/store-products:1.0.0.
2- Create a service of NodePort to expose this deployment outside the host. 
3- Test that you can open the web app from outside the host using the host IP address and port.

# Environment
Ubuntu VM on VMWare workstation
# Tools

minikube

Docker hub to get the image (linuxacademycontent/store-products:1.0.0)

# Commands

First To create deployment:
  kubectl apply deployment-defintion.yml

Second is to expose NodePort
  kubectl expose deployment deploy-replicas --type=NodePort --port=80
