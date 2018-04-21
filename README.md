

## deploy k8s cluster using ansible
```
rm -rf *.retry

ansible-playbook -vvvv -i hosts 01.prepare.yml

ansible-playbook -vvvv -i hosts 02.etcd.yml

#ansible-playbook -vvvv -i hosts 03.docker.yml

ansible-playbook -vvvv -i hosts 03.docker-image.yml

ansible-playbook -vvvv -i hosts 04.kube-master.yml

ansible-playbook -vvvv -i hosts 05.kube-node.yml

ansible-playbook -vvvv -i hosts 06.network.yml

ansible-playbook -vvvv -i hosts 07.kube-plugin.yml
```




## kubernetes binaries
```
10.12.0.100 /root/kubernetes_binary/*


v1.10.0-rc.1  v1.6.12  v1.6.13  v1.7.1  v1.7.10  v1.7.15  v1.8.0  v1.8.10  v1.8.4  v1.8.6  v1.9.0  v1.9.1  v1.9.2  v1.9.3  v1.9.4  v1.9.5
```



## reference

* ansible for kubernetes using binary style
```
https://github.com/gjmzj/kubeasz
```

* resources reserved
```
https://kubernetes.io/docs/tasks/administer-cluster/reserve-compute-resources/#kube-reserved
```

* bianry download
```
https://github.com/kubernetes/kubernetes/releases
```

* 
