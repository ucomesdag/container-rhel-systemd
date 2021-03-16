Red Hat Universal Base Image with Systemd
=====================

This Containerfile can build containers capable to use systemd.

[![rhel build status](https://quay.io/repository/ucomesdag/rhel/status "Container Repository on Quay")](https://quay.io/repository/ucomesdag/rhel)

Branches
--------

This repository has multiple branches that relate to RedHat versions.

|Branch |RHEL Version|Container image tag|
|-------|------------|-------------------|
|main   |latest (8)  |latest             |

Pull strategy
-------------

The different branches are **not** merged, they live as individual branches.

Manually starting
-----------------

```
podman run \
  --tty \
  --privileged \
  --volume /sys/fs/cgroup:/sys/fs/cgroup:ro \
  quay.io/ucomesdag/rhel
```
