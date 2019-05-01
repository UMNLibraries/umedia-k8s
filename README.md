
# Experimental

This is a kubernetes learning project.

# Deploy
* Install kubernetes (e.g. via [minikube](https://kubernetes.io/docs/setup/minikube/))
* Expose the Rails `SECRET_KEY_BASE` to the cluster
  * `$ kubeclt create secret generic SECRET_KEY_BASE --from-literal SECRET_KEY_BASE=<your value here>`
* Configure the cluster (from the `umedia-k8s` directory:
  * `kc apply -f .`