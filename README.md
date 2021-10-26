# Developer Notes

Original repo: `https://github.com/jonathanbaraldi/devops`

Demo: `https://github.com/jchengdev/k8s-sample-gke`

## Ignore List

- "Aula 9" replaced with scripts from other sources

## Command List

- (cluster creation and kubeconfig setup)
- `kubectl create ns traefik-system`
- `helm repo add traefik https://helm.traefik.io/traefik`
- `helm repo update`
- `helm install --namespace=traefik-system traefik-ingress-controller traefik/traefik`
- `kubectl get svc -n traefik-system`
- `kubectl port-forward $(kubectl get pods --selector "app.kubernetes.io/name=traefik" --output=name -n traefik-system | head -n 1) 9000:9000 -n traefik-system`
- `kubectl apply -f ./kubectl_commands_N_files/traefik_dashboard.yml`
- (fix nodes driver issue: GKE with Ubuntu-containerd OS image)
- `kubectl create clusterrolebinding cluster-admin-binding --clusterrole=cluster-admin --user=<my@email.com>`
- (longhorn installation via Apps & Marketplace)
