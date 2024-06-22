# Create Hetzner cloud vms with ansible

Just loading those 2 Playbooks here off.

### example host_var

```
hetzner:
    project: "serious-project"
    server_type: "cpx11"
    image: "fedora-38"
    zone: "example.com"
    location: "fsn1"
    ipv6: True
    ttl: 300
    key_names:
      - "ford-prefect@earth"
```

