https://opensource.com/article/20/5/kubectl-cheat-sheet


Install k3s https://k3s.io/  
`curl -sfL https://get.k3s.io | sh -`  

`kubectl get pods --all-namespaces`

Docker Desktop for Mac  
`kubectl config use-context docker-desktop`

Shell into pod  
`kubectl exec --stdin --tty PODNAME -- /bin/bash`

Change default namespace  
`kubectl config set-context --current --namespace=<insert-namespace-name-here>`    
Validate it  
`kubectl config view --minify | grep namespace:`