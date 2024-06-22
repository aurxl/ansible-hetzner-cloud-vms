# Create Hetzner cloud vms with ansible

Just loading those 2 Playbooks here off.

### example host_var

```yaml
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

### example goup_var
```yaml
projects:
  serious_project:
    hetzner_api_token: !vault |
      $ANSIBLE_VAULT;1.1;AES256
      1234...

  other_project:
    hetzner_api_token: !vault |
      $ANSIBLE_VAULT;1.1;AES256
      1234..

hetzner_dns_api: !vault |
  $ANSIBLE_VAULT;1.1;AES256
  1234...
```

