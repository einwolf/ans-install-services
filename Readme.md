# Install services

Install various services

## Grafana with Prometheus

```bash
reset && ansible-playbook -v -l gpdash install-gpdash.yaml -b -k -K
```

## Monitors

```bash
reset && ansible-playbook -v -l ne install-ne.yaml -b -k -K
```
