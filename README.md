# sdeNow
inf-cli exec -i -n kube-system $(inf-cli get pods -a |  awk '/ec-system/{print $2}') kube-apiserver -- /bin/bash

crx-cli exec list

stty cols 132

kubectl --kubeconfig /etc/kubernetes/admin.conf get pods --all-namespaces

kubectl --kubeconfig /etc/kubernetes/admin.conf top pods --all-namespaces

kubectl --kubeconfig /etc/kubernetes/admin.conf get events --all-namespaces

kubectl --kubeconfig /etc/kubernetes/admin.conf describe pod <pod name> -n <namespace>

kubectl --kubeconfig /etc/kubernetes/admin.conf exec -it <pod name> -n <namespace> -- /bin/bash
