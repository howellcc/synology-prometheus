## Dependencies
- [Synology Docker](https://www.synology.com/en-global/dsm/packages/Docker) package already installed.
- SSH access to synology.
- Administrator user access.
- In docker on synology there is a "container_network" bridge network setup


### Install
```bash
curl --no-sessionid -fsSL https://raw.githubusercontent.com/howellcc/synology-prometheus/ForMe/setup | sudo sh
```

### Uninstall
```bash
curl --no-sessionid -fsSL https://raw.githubusercontent.com/howellcc/synology-prometheus/ForMe/uninstall | sudo sh
```

#### Endpoints
- Grafana `http://<synology ip/hostname>:3000` (this may take upto 15 seconds to start up.)
- Prometheus `http://<synology ip/hostname>:9090`
- Alertmanager `http://<synology ip/hostname>:9093`
- Node-Exporter `http://<synology ip/hostname>:9100/metrics`
