# Oracle Database Helm Chart

This helm chart is for my personal homelab but very easy to customize to your own.

It spins up an Oracle Database using the Oracle XE 21c Image, which is free and has a click-through
license. It mounts it to an NFS Share and use a Traefik `IngressRouteTCP` to direct ingress.

# Install

```bash
helm upgrade --install oracle-db -f charts/oracle-db/values.yaml charts/oracle-db --namespace oracle-namespace
```


# TODO

A lot of todo here...

- Make the templating must more extendable
- Documentation on how to use, making edits, etc.
- Probably leverage the `faststart` images for a quick database