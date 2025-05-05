# Kubernetes Manifests Project

This project contains Kubernetes manifests for deploying and managing resources in a Kubernetes cluster.

## Project Structure

```
manifests/
    configmap.yaml      # Kubernetes ConfigMap definition
    deployment.yaml     # Kubernetes Deployment definition
    namespace.yaml      # Kubernetes Namespace definition
    service.yaml        # Kubernetes Service definition
```

## Files Description

- **manifests/configmap.yaml**: Defines configuration data that can be consumed by pods in the cluster.
- **manifests/deployment.yaml**: Specifies the desired state for a set of pods and their replicas.
- **manifests/namespace.yaml**: Declares a namespace to isolate resources within the cluster.
- **manifests/service.yaml**: Describes a Kubernetes Service to expose pods to other services or external traffic.

## Usage

1. Apply the manifests to your Kubernetes cluster using `kubectl`:
   ```sh
   kubectl apply -f manifests/
   ```

2. Verify the resources have been created:
   ```sh
   kubectl get all --namespace=<namespace-name>
   ```

## License

This project is licensed under the MIT License.