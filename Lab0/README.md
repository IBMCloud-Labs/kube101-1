# Lab 0. Set up your kubernetes environment

For the hands-on labs in this tutorial repository, you will need a kubernetes cluster. You can either create one as-a-service from the IBM Cloud Kubernetes Service, use a hosted environment or install one locally on your workstation.

## Use the IBM Cloud Kubernetes Service

You will need either a paid IBM Cloud account or an IBM Cloud account which is a Trial account (not a Lite account). If you have one of these accounts, use the [Getting Started Guide](https://cloud.ibm.com/docs/containers?topic=containers-getting-started) to create your cluster.

## Use a hosted trial environment

There are a few services that are accessible over the Internet for temporary use. As these are free services, they can sometimes experience periods of limited availablity/quality. On the other hand, they can be a quick way to get started!

* [Kubernetes playground on Katacoda](https://www.katacoda.com/courses/kubernetes/playground) This environment starts with a master and worker node pre-configured. You can run the steps from Labs 1 and onward from the master node.

* [Play with Kubernetes](https://labs.play-with-k8s.com/) After signing in with your github or docker hub id, click on **Start**, then **Add New Instance** and follow steps shown in terminal to spin up the cluster and add workers.

## Set up on your own workstation

If you would like to configure kubernetes to run on your local workstation for non-production, learning use, there are several options.

* [Minikube](https://kubernetes.io/docs/setup/learning-environment/minikube/) This solution requires the installation of a supported VM provider (KVM, VirtualBox, HyperKit, Hyper-V - depending on platform)

* [Kubernetes in Docker (kind)](https://kind.sigs.k8s.io/) Runs a kubernetes cluster on Docker containers

* [Docker Desktop (Mac)](https://docs.docker.com/docker-for-mac/kubernetes/) [Docker Desktop (Windows)](https://docs.docker.com/docker-for-windows/kubernetes/) Docker Desktop includes a kubernetes environment

* [Microk8s](https://microk8s.io/docs/) Installable kubernetes packaged as an Ubuntu `snap` image.

## Instructions for those with provided web terminal and cluster
**Interact With Your Cluster From Provided Web Terminal** 

Note: In the provided web terminal, the CLI downloads required will be provided. 

1. Sign into www.cloud.ibm.com. Please use guest network or hotspot your phone if you can not get to this website due to firewall for this step. 
2. Navigate to the left hand side hamburger menu in top left, then click on “dashboard” in the drop-down menu. 
![](https://paper-attachments.dropbox.com/s_878C1E366CE3BC0E7C5F83D7C1CA600E85849877C47E2C809FD98306260E211F_1566423075745_Screen+Shot+2019-08-21+at+12.42.07+PM.png)

3. Click on “Kubernetes cluster” where we have provisioned one cluster per web terminal.  Locate your cluster provisioned using **the same number** you have been assigned by web terminal. If I am web terminal 17, I’ll use kubernetes cluster 17, for example.  Click on your numbered cluster. 
![](https://paper-attachments.dropbox.com/s_878C1E366CE3BC0E7C5F83D7C1CA600E85849877C47E2C809FD98306260E211F_1566423119116_Screen+Shot+2019-08-21+at+12.27.36+PM.png)

4. Now you will see your cluster details and status. Click on the blue button “connect with CLI.”  Copy and paste the CLI commands to login, and configure your cluster. **Note:** **Do not forget to export** your KUBECONFIG as an environment variable, and copy the output provided from step 2 into your terminal. 
![](https://paper-attachments.dropbox.com/s_878C1E366CE3BC0E7C5F83D7C1CA600E85849877C47E2C809FD98306260E211F_1566423366687_Screen+Shot+2019-08-21+at+12.27.53+PM.png)

## Helpful links 

1. Graphs and explanation of Kubernetes in more detail: https://github.com/IBM/kube101/tree/master/workshop
2. Kubernetes explained video: https://www.youtube.com/watch?v=aSrqRSk43lY
