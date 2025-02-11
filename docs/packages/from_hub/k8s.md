# k8s
### Visit the package [ Source Code ](https://github.com/cocmd/hub/tree/master/packages/k8s)
> Please contribute your k8s playbooks and shortcuts
> [How to contribute?](https://github.com/cocmd/hub/blob/master/CONTRIBUTING.md)
:::info How To Install?
run in terminal:
```bash
cocmd install -y k8s
```
:::
## automations (5)
| command | env | description | how to run? |
| --- | --- | --- | --- |
| k8s.setup | MacOS | setup Kubernetes for desktop: Instructions. Install Kubectl. Install Kubectx. Install Minikube. Intall K9s - Kubernetes CLI To Manage Your Clusters In Style. Install Helm. Install kube-capacity. Install Kor - Kubernetes Orphaned Resources Finder. Install kubefwd. Install VSCode plugins.  | run `k8s.setup` or `cocmd run k8s.setup` |
| k8s.setup | Linux | Setup Kubernetes for desktop on Linux: Instructions. Install Kubectl. Install Kubectx. Install Minikube. Install Helm. Install VSCode plugins.  | run `k8s.setup` or `cocmd run k8s.setup` |
| k8s.backup-configmaps | Any | Backup all ConfigMaps in a namespace | run `k8s.backup-configmaps` or `cocmd run k8s.backup-configmaps` |
| k8s.rolling-restart | Any | Perform a rolling restart of a Deployment | run `k8s.rolling-restart` or `cocmd run k8s.rolling-restart` |
| k8s.batch-pod-deletion | Any | Batch delete Pods based on a label | run `k8s.batch-pod-deletion` or `cocmd run k8s.batch-pod-deletion` |
| k8s.check-pod-restarts | Any | Check for Pods with restart counts greater than 0 | run `k8s.check-pod-restarts` or `cocmd run k8s.check-pod-restarts` |

## aliases (125):
```
alias k='kubectl'
alias kl='kubectl logs'
alias kexec='kubectl exec -it'
alias kpf='kubectl port-forward'
alias kaci='kubectl auth can-i'
alias kat='kubectl attach'
alias kapir='kubectl api-resources'
alias kapiv='kubectl api-versions'

# get
alias kg='kubectl get'
alias kgns='kubectl get ns'
alias kgp='kubectl get pods'
alias kgs='kubectl get secrets'
alias kgd='kubectl get deploy'
alias kgrs='kubectl get rs'
alias kgss='kubectl get sts'
alias kgds='kubectl get ds'
alias kgcm='kubectl get configmap'
alias kgcj='kubectl get cronjob'
alias kgj='kubectl get job'
alias kgsvc='kubectl get svc -o wide'
alias kgn='kubectl get no -o wide'
alias kgr='kubectl get roles'
alias kgrb='kubectl get rolebindings'
alias kgcr='kubectl get clusterroles'
alias kgrb='kubectl get clusterrolebindings'
alias kgsa='kubectl get sa'
alias kgnet='kubectl get netpol'

# edit
alias ke='kubectl edit'
alias kens='kubectl edit ns'
alias kes='kubectl edit secrets'
alias ked='kubectl edit deploy'
alias kers='kubectl edit rs'
alias kess='kubectl edit sts'
alias keds='kubectl edit ds'
alias kesvc='kubectl edit svc'
alias kecm='kubectl edit cm'
alias kecj='kubectl edit cj'
alias ker='kubectl edit roles'
alias kerb='kubectl edit rolebindings'
alias kecr='kubectl edit clusterroles'
alias kerb='kubectl edit clusterrolebindings'
alias kesa='kubectl edit sa'
alias kenet='kubectl edit netpol'

# describe
alias kd='kubectl describe'
alias kdns='kubectl describe ns'
alias kdp='kubectl describe pod'
alias kds='kubectl describe secrets'
alias kdd='kubectl describe deploy'
alias kdrs='kubectl describe rs'
alias kdss='kubectl describe sts'
alias kdds='kubectl describe ds'
alias kdsvc='kubectl describe svc'
alias kdcm='kubectl describe cm'
alias kdcj='kubectl describe cj'
alias kdj='kubectl describe job'
alias kdsa='kubectl describe sa'
alias kdr='kubectl describe roles'
alias kdrb='kubectl describe rolebindings'
alias kdcr='kubectl describe clusterroles'
alias kdcrb='kubectl describe clusterrolebindings'
alias kdnet='kubectl describe netpol'

# delete
alias kdel='kubectl delete'
alias kdelns='kubectl delete ns'
alias kdels='kubectl delete secrets'
alias kdelp='kubectl delete po'
alias kdeld='kubectl delete deployment'
alias kdelrs='kubectl delete rs'
alias kdelss='kubectl delete sts'
alias kdelds='kubectl delete ds'
alias kdelsvc='kubectl delete svc'
alias kdelcm='kubectl delete cm'
alias kdelcj='kubectl delete cj'
alias kdelj='kubectl delete job'
alias kdelr='kubectl delete roles'
alias kdelrb='kubectl delete rolebindings'
alias kdelcr='kubectl delete clusterroles'
alias kdelrb='kubectl delete clusterrolebindings'
alias kdelsa='kubectl delete sa'
alias kdelnet='kubectl delete netpol'

# mock
alias kmock='kubectl create mock -o yaml --dry-run=client'
alias kmockns='kubectl create ns mock -o yaml --dry-run=client'
alias kmockcm='kubectl create cm mock -o yaml --dry-run=client'
alias kmocksa='kubectl create sa mock -o yaml --dry-run=client'

# config
alias kcfg='kubectl config'
alias kcfgv='kubectl config view'
alias kcfgns='kubectl config set-context --current --namespace'
alias kcfgcurrent='kubectl config current-context'
alias kcfggc='kubectl config get-contexts'
alias kcfgsc='kubectl config set-context'
alias kcfguc='kubectl config use-context'
alias kcfgv='kubectl config view'

# Kubescape related
alias kssbom='kubectl -n kubescape get sbomspdxv2p3s'
alias kssbomf='kubectl -n kubescape get sbomspdxv2p3filtereds'
alias kssboms='kubectl -n kubescape get sbomsummaries'
alias ksvulns='kubectl -n kubescape get vulnerabilitymanifestsummaries'
alias ksvuln='kubectl -n kubescape get vulnerabilitymanifests'

# Kubescape related with labels
alias kssboml='kubectl -n kubescape get sbomspdxv2p3s --show-labels'
alias kssbomfl='kubectl -n kubescape get sbomspdxv2p3filtereds --show-labels'
alias kssbomsl='kubectl -n kubescape get sbomsummaries --show-labels'
alias ksvulnsl='kubectl -n kubescape get vulnerabilitymanifestsummaries --show-labels'
alias ksvulnl='kubectl -n kubescape get vulnerabilitymanifests --show-labels'

alias m='minikube'
alias ma='minikube addons'
alias ms='minikube service'
alias minid='minikube delete'
alias minis='minikube start'
alias miniv='minikube version'

```

