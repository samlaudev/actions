# Kubernetes gcr.io images sync

This action for syncing kubernetes gcr.io images

## Inputs

### `username`

**Required** Username used to login docker registry. 

### `password`

**Required** Password used to login docker registry.

### `registry`

Docker registry server address. Default `''`

### `owner`

**Required** docker image owner name. 

### `kubernetes_version`

set kubernetes version



## Example usage

uses: samlaudev/actions/k8s-image-sync@master
with:
  username: ${{ secrets.DOCKER_USERNAME }}

  password:  ${{ secrets.DOCKER_PASSWORD }}

  owner: ${{ secrets.DOCKER_USERNAME }}

  kubernetes_version: v1.14.8 