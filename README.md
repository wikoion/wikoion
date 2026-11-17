# Richard Draycott

Senior Software Engineer on the platform team at InfluxData, based in Seattle. Most of my work is Kubernetes, Cluster API and node autoscaling, mostly in Go and Rust. Nearly all of it lives in private repos, so this page is the public bits.

## capi-autoscaler

[capi-autoscaler](https://github.com/wikoion/capi-autoscaler) is my MSc Computer Science project. It's a Cluster API autoscaler that treats scale-up as a bin-packing problem, solves it with OR-Tools CP-SAT, then uses scheduling gates to steer pods onto the nodes it planned for.

I benchmarked it against Cluster Autoscaler and Karpenter on EC2. It had the highest CPU utilisation in all nine scenarios and a lower estimated fleet cost than both wherever they completed. Karpenter was faster to scale up in every scenario. The data and the notebook that produces every number are in [capi-autoscaler-research](https://github.com/wikoion/capi-autoscaler-research).

The public repo is a single squashed commit. Development happened in a private repo from Jan 2026 to September 2026.

## Older stuff

Personal projects from 2018 to 2022 are on GitLab. The main one is a Go blog API on MongoDB and Elasticsearch with a ClojureScript front end, run with docker compose across two Raspberry Pis and later deployed with Helm. There's also a Spring Boot blog and Ansible for installing Arch on ZFS.

- [wikoion-dev-projects](https://gitlab.com/wikoion-dev-projects)
- [system-configuration-files](https://gitlab.com/system-configuration-files)

## Other bits

Side projects outside work: [strap-sync](https://github.com/wikoion/strap-sync) reads a WHOOP strap over Bluetooth and writes to Apple Health, [tare](https://github.com/wikoion/tare) is an app for Etekcity smart scales, and [switchboard-oss](https://github.com/wikoion/switchboard-oss) is a self-hosted Matrix chat inbox.
