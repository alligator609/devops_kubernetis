## why kubernetes

1. if a container die we have to manually start the container. And no way to know if the container died or not.
2. if we need 100 container containing same application how can we manage that??


## kubernetere

### control plane
1. master node
    * kubectl (cli)
    * API server which communicate with kubelet also comands of kubectl. Save data to ETCD. 
    * ETCD hich save data through APIserver. 
    * Scheduler 

note: i need a python caontainer   

### dataplane
    * worker node 1 (kubelet will manage worker if running or not)
    * worker node 2 (kubelet will manage worker if running or not)
    


## keywords
1. Deployment ( Don't let the pods to die)
2. Pod (1 or multiple container)
3. Service (Sends traffic to pods)
    three types of service 
    * load balancer
    * node port 
    * cluster IP 

## how service mange pods

by Labels & Selector. Service labe;  inside service


### books
1. kubernetes action