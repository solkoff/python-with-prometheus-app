# Metrics that we can expose in Grafana

## Overview of metric

1. `running_pods` is a Gauge metric, and shows the total # of running pods in Kubernetes. It leverages a Python library to interrogate the Kubernetes API, and then filters by Status to return a count of running pods in your Kubernetes cluster.
2. `app_hello_world_total` is a Counter metric, and increments each time the `https://localhost:5000` endpoint is hit.
3. `count:up1` -> metrics of number of pods of that application

The metrics are exposed at "/metrics" ednpoint