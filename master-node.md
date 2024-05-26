The Kubernetes Master Node is the control plane that manages the Kubernetes cluster.

# Kubernetes Master Node Components

## 1. API Server (kube-apiserver)
- **Description**: Acts as the front end for the Kubernetes control plane.
- **Function**: Handles RESTful API requests, validates them, and processes them.

## 2. etcd
- **Description**: A consistent and highly-available key-value store used as Kubernetes' backing store.
- **Function**: Stores all cluster data, including configuration details and the current state of the cluster.

## 3. Scheduler (kube-scheduler)
- **Description**: Responsible for distributing workload across the cluster.
- **Function**: Assigns newly created pods to nodes based on resource availability and other constraints.

## 4. Controller Manager (kube-controller-manager)
- **Description**: Runs various controllers to regulate the state of the cluster.
- **Function**: Includes node controller, replication controller, and others to ensure the desired state of the cluster matches the actual state.

## 5. Cloud Controller Manager (cloud-controller-manager)
- **Description**: Manages cloud-specific control logic.
- **Function**: Interacts with the underlying cloud service provider to handle node management, load balancing, and other cloud-specific resources.

These components work together to ensure the Kubernetes cluster operates efficiently and remains resilient.
