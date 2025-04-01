# Alloy --> Runit service

Grafana Alloy is a service that acts as an agent to collect
**metrics**, **logs**, **traces**, and **profiles** from the host system.
It forwards this telemetry data to the appropriate backends.

The service requires the following environment variables to be set in order to reach
the corresponding databases:

```bash
export LOKI_HOST="YOUR LOKI HOST"
export REMOTE_WRITE_HOST="YOUR MIMIR HOST"
export TEMPO_HOST="YOUR TEMPO HOST"
export PYROSCOPE_HOST="YOUR PYROSCOPE HOST"
```

Grafana Alloy runs as a system-level service.
Its default configuration is available in the [alloy directory](../../config/alloy/README.md).

Make sure to customize the configuration and environment variables
according to your infrastructure.
