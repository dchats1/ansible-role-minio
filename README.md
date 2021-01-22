MinIO
=========

This role deploys MinIO in Podman Containers.

Requirements
------------

This requires the containers.podman collection: https://galaxy.ansible.com/containers/podman

Role Variables
--------------

Variable                   | Description
---------------------------|------------------------------------------
minio_mode                 | Mode to run MinIO. Either standard or erasure-code. (Default: standard)
minio_access_key           | Access Key (Default: AKIAIOSFODNN7EXAMPLE)
minio_secret_key           | Secret Key (Default: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY)
minio_podman_network       | Podman network to run the container on. (Default: podman)
minio_hostname             | Hostname for the pod. (Default: minio)
minio_domain               | Domain for the pod. (Default: example.com)
minio_prometheus_auth_type | Type of auth to use for prometheus metrics. Either jwt or public. (Default: jwt)


Example Playbook
----------------

```
 - hosts: minio
   roles:
      - minio
```

License
-------

BSD

Author Information
------------------

David Chatterton
david@davidchatterton.com
