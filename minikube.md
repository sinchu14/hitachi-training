1. Check minikube is working 

minikube status

minikube stop

minikube delete --purge 

~/.minikube --> certificates, configs and profile 

rm -f /usr/local/bin/minikube

2. To install , once minikube is downloaded 

install minikube-linux-amd64 /usr/local/bin/minikube

3 - If you find any issues with /tmp/juju-* 

  rm -f /tmp/juju-*

  sysctl fs.protected_regular=0

4- Install kubectl 

    https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/
