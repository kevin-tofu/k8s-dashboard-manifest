## Kubernetes Dashboard Manifest File  

#### Microk8s Environment

```
microk8s enable dashboard dns
```

```
microk8s.kubectl port-forward -n kube-system service/kubernetes-dashboard --address 0.0.0.0 10443:443 &
```

```
microk8s.kubectl apply -f dashboard-account.yml
```

```
microk8s.kubectl describe secrets dashboard-admin -n kube-system
```


