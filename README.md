
# Developer Notes

Ongoing demo creation

Original repo: `https://github.com/jonathanbaraldi/devops`

## Ignore List

- "Aula 9" replaced with scripts from other sources

## Command List

- `kubectl create ns traefik-system`
- `kubectl apply -f ./kubectl_commands_N_files/traefik_rbac.yml`
- `kubectl apply -f ./kubectl_commands_N_files/traefik_system_svc.yml`
- `kubectl describe -n traefik-system ds/traefik-ingress-controller`
- `kubectl get svc -n traefik-system`
- (fix nodes driver issue: GKE with Ubuntu-containerd OS image)
- `kubectl create clusterrolebinding cluster-admin-binding --clusterrole=cluster-admin --user=<my@email.com>`
- (longhorn installation via Apps & Marketplace)
