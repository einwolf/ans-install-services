# Install services

Install various services

```bash
ANSIBLE_HOST_KEY_CHECKING=false ansible-playbook -v ping.yaml -l dashboard,ne_clients
```

## Grafana with Prometheus

```bash
reset && ansible-playbook -v install-graphdash.yaml -b -k -K
reset && ansible-playbook -v install-graphdash.yaml -l graphdash
```

## Monitors

```bash
reset && ansible-playbook -v install-node_exporter.yaml -l nodebox1 -b -k -K
reset && ansible-playbook -v install-node_exporter.yaml -l nodebox1
```
