MinIO
=========

This role deploys MinIO on Podman Containers.

Requirements
------------

This requires the containers.podman collection: https://galaxy.ansible.com/containers/podman

Role Variables
--------------

Variable              | Description
----------------------|------------------------------------------
minio_access_key      | Access Key (Default: AKIAIOSFODNN7EXAMPLE"_
minio_secret_key      | Secret Key (Default: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY)
minio_mode            | Mode to run MinIO. Options: standalone, distributed (not yet implemented) (Default: standalone)
minio_podman_network  | Podman network to run the container on. (Default: podman)
minio_hostname        | Hostname for the pod. (Default: minio)
minio_domain          | Domain for the pod. (Default: example.com)


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
