# wittdennis.kubeadm_upgrade

Ansible role to upgrade nodes of a kubeadm Kubernetes cluster

## Requirements

In order to send drain and (un)cordon commands tasks need to be delegated to a kubernetes control plane. This role assumes you have a `kubernetes_control_plane` group in your inventory.

## Role Variables

```yaml
---
kubeadm_upgrade_kubernetes_version: v1.30.3
```

## Example Playbook

    - hosts: servers
      roles:
         - { role: wittdennis.kubeadm_upgrade }

## License

MIT
