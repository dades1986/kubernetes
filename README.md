# kubernetes
# Getting Started with Kubernetes

## Notes and Concepts

### 1. Kubernetes Basics:
- **Pods:** Smallest deployable units in Kubernetes that can hold one or multiple containers.
- **Nodes:** Worker machines in Kubernetes.
- **Clusters:** A set of worker machines (nodes) that run containerized applications.
- **Kubectl:** Command-line tool for interacting with a Kubernetes cluster.
- **Kubelet:** Agent running on each node in the cluster.
- **API Server:** Front-end to the cluster's control plane.
- **Etcd:** Consistent and highly-available key-value store used as Kubernetes' backing store.
- **Control Plane:** Collection of processes that control Kubernetes nodes.
- **Namespace:** Virtual clusters backed by the same physical cluster.

### 2. Workloads & Controllers:
- **Deployments:** Manages a replicated application.
- **ReplicaSets:** Ensures a specified number of replicas of a Pod are running.
- **StatefulSets:** Manages deployment and scaling of a set of Pods with guarantees about ordering and uniqueness.
- **DaemonSets:** Ensures all (or some) nodes run a copy of a Pod.
- **Jobs:** Creates one or more Pods and ensures a specified number of them successfully terminate.
- **CronJobs:** Manages time-based Jobs, such as running a Job at specific times or intervals.
- **Horizontal Pod Autoscaler:** Scales Pods based on observed CPU or memory usage.

### 3. Services & Networking:
- **Services:** Exposes an application running in Pods as a network service.
- **Ingress:** Manages external access to services within a cluster.
- **Network Policies:** Define how Pods communicate with each other securely.
- **Service Discovery:** Mechanism to connect to services dynamically based on a logical name.
- **Load Balancer:** Distributes network traffic across multiple Pods.

### 4. Configuration & Secrets:
- **ConfigMaps:** Manage configuration data separately from container images.
- **Secrets:** Manages sensitive information, such as passwords and API keys.
- **Environment Variables:** Used within Kubernetes for service discovery.
- **Volumes:** Persistent storage in Kubernetes.
- **Persistent Volume Claims (PVCs):** Request for storage by a user.

### 5. Monitoring, Logging, and Debugging:
- **Kube-state-metrics:** Generates metrics about the state of Kubernetes objects.
- **Prometheus:** System monitoring and alerting toolkit.
- **Grafana:** Platform for analytics and monitoring.
- **ELK Stack:** Elasticsearch, Logstash, and Kibana for logging.
- **Kubernetes Dashboard:** Web UI for Kubernetes clusters.
- **Kubectl Debug:** Tool for debugging Pods.
- **Heapster:** Collects monitoring and performance metrics.

### 6. Security & Authorization:
- **Role-Based Access Control (RBAC):** Access control system.
- **Security Policies:** Constraints applied to a Pod for security.
- **Service Account:** Identity attached to Pods to interact with the Kubernetes API Server.
- **Transport Layer Security (TLS):** Protocol for privacy and data integrity.

### 7. Kubernetes Storage:
- **Persistent Volumes (PVs):** Offers storage to the cluster independent of Pod lifecycles.
- **Storage Classes:** Describes classes of storage offered to Kubernetes.

### 8. Kubernetes Cluster Maintenance:
- **Node Maintenance:** Taking nodes down for maintenance or replacing failing nodes.
- **Cluster Upgrades:** Upgrading the cluster to a newer version.
- **Backup and Disaster Recovery:** Ensuring data continuity and integrity.

### 9. Extending Kubernetes:
- **Custom Resources:** Extension of the Kubernetes API.
- **API Server Extension:** Custom endpoints in the Kubernetes API.
- **Custom Controllers:** Automates handling of Custom Resources.
- **Operators:** Application-specific controllers for complex stateful applications.

### 10. Advanced Features:
- **Service Mesh (e.g., Istio):** Manages microservices in a transparent way.
- **Pod Priority & Preemption:** Specifies priorities for Pods and allows preemption of lower-priority Pods.
- **Taints and Tolerations:** Allows a node to repel a set of Pods.
- **Node Affinity:** Controls where a Pod runs based on labels on nodes and conditions.
- **Pod Presets:** Injects information into Pods at creation time.

### 11. Kubernetes Cloud Integration:
- **Amazon EKS:** Managed Kubernetes service on AWS.
- **Google Kubernetes Engine (GKE):** Managed Kubernetes service on Google Cloud.
- **Azure AKS:** Managed Kubernetes service on Azure.

### 12. Continuous Deployment/Integration in Kubernetes:
- **Jenkins:** Continuous integration and build automation.
- **GitLab CI:** Continuous integration service included with GitLab.
- **Spinnaker:** Continuous delivery platform for releasing software changes.

### 13. Helm: Kubernetes Package Manager:
- **Helm Charts:** Packages of pre-configured Kubernetes resources.
- **Helm Repository:** Collection of charts for Kubernetes packages.

### 14. Kubernetes Custom Scheduling:
- **Custom Scheduler:** Control over the scheduling of Pods.

### 15. Kubernetes Federation:
- **Cluster Federation:** Synchronizes resources across multiple clusters.

### 16. Windows in Kubernetes:
- **Windows Nodes:** Support for Windows worker nodes and containers in Kubernetes.

### 17. Kubernetes Testing:
- **Kubetest:** End-to-end testing for Kubernetes.

### 18. Kubernetes Add-ons:
- **DNS:** DNS server for service name resolution.
- **Web UI (Dashboard):** Web-based Kubernetes user interface.
- **Container Resource Monitoring:** Time-series monitoring of resource utilization.
- **Cluster-level Logging:** Save container logs to a logging backend.

### 19. Other Essential Concepts:
- **Quotas:** Constraints applied to resources like Pods and Persistent Volumes.
- **Annotations:** Attach metadata to Kubernetes objects.
- **Labels and Selectors:** Key/value pairs and selection criteria for objects.
- **Liveness and Readiness Probes:** Health checks for applications.

### 20. Kubernetes Failure Handling:
- **Pod Disruption Budgets (PDBs):** Constraints on voluntary disruptions for Pods.

### 21. Kubernetes Architecture Concepts:
- **Cloud Controller Manager:** Embeds cloud-specific logic for the provider.
- **Kube-Proxy:** Maintains network rules and enables connection forwarding.
- **Container Runtime:** Software to run containers, e.g., Docker, containerd.

### 22. Kubernetes Community and Development:
- **Special Interest Groups (SIGs):** Kubernetes project divisions.
- **Contributing to Kubernetes:** Guide to contributing to the Kubernetes project.

### 23. Kubernetes Best Practices:
- **Logging Best Practices:** Guidelines for logging in Kubernetes.
- **Monitoring Best Practices:** Guidelines for monitoring Kubernetes.
- **Security Best Practices:** Guidelines for securing applications in Kubernetes.
- **Performance Best Practices:** Guidelines for optimal Kubernetes performance.

### 24. Kubernetes Automation and Autoscaling:
- **Cluster Autoscaler:** Automatically adjusts cluster size.
- **Vertical Pod Autoscaler:** Adjusts CPU and memory requested by containers.
- **Horizontal Pod Autoscaler (HPA):** Scales Pods based on CPU or memory usage.

### 25. Kubernetes Development Tools:
- **Minikube:** Runs a single-node Kubernetes cluster on your laptop.
- **Skaffold:** Facilitates continuous development for Kubernetes applications.
- **Kompose:** Converts Docker Compose files to Kubernetes.
- **Kubeadm:** Tool for bootstrapping a Kubernetes cluster.

### 26. Advanced Kubernetes Networking:
- **Network Plugins:** Extend Kubernetes networking capabilities.
- **CNI (Container Network Interface):** Standard for configuring network interfaces in Linux containers.
- **Flannel:** Overlay network provider.
- **Calico:** Provides secure network connectivity.

### 27. Kubernetes Performance Tuning:
- **Kubelet Garbage Collection:** Cleanup of unused images or containers.
- **Kernel Tuning:** Adjusting Linux kernel parameters for performance optimization.

### 28. Kubernetes Service Mesh:
- **Istio:** Connects, manages, and secures microservices.
- **Linkerd:** Service mesh for Kubernetes.

### 29. Kubernetes Mobile Integration:
- **Kubernetes on Edge:** Running Kubernetes in edge computing environments.

### 30. Additional Kubernetes Ecosystem Tools:
- **Cilium:** Security and networking for cloud-native applications.
- **Knative:** Platform to build, deploy, and manage modern serverless workloads.
- **OpenFaas:** Function as a Service (FaaS) platform on Kubernetes.
- **Metacontroller:** Creates custom controllers using simple scripting languages.

## Kubernetes Commands & Usages:

### 1. Basic Cluster Information:
- `kubectl cluster-info`: Display information about the cluster.
- `kubectl version`: Display version info.

### 2. Working with Nodes and Cluster:
- `kubectl get nodes`: List nodes in a cluster.
- `kubectl describe node <node-name>`: Show details of a specific node.

### 3. Working with Pods:
- `kubectl get pods`: List all pods in all namespaces.
- `kubectl run <name> --image=<image>`: Deploy a new Pod with a given image.
- `kubectl describe pod <pod-name>`: Describe a specific pod.
- `kubectl logs <pod-name>`: Fetch the logs from a pod.
- `kubectl delete pod <pod-name>`: Delete a specific pod.

### 4. Working with Deployments:
- `kubectl create deployment <name> --image=<image>`: Create a new deployment.
- `kubectl get deployments`: List all deployments.
- `kubectl describe deployment <deployment-name>`: Describe a specific deployment.
- `kubectl scale deployment <deployment-name> --replicas=<num>`: Scale up/down a deployment.

### 5. Working with Services:
- `kubectl expose deployment <name> --type=LoadBalancer --port
8080: Expose a deployment as a service.
- `kubectl get services`: List all services.
- `kubectl describe service <service-name>`: Describe a specific service.

### 6. Config and Storage:
- `kubectl get configmaps`: List all config maps.
- `kubectl create configmap <name> --from-file=<path>`: Create a config map from a file.
- `kubectl get secrets`: List all secrets.
- `kubectl create secret`: Create a secret.
- `kubectl get pv`: List all persistent volumes.
- `kubectl get pvc`: List all persistent volume claims.

### 7. Namespaces and Context:
- `kubectl get namespaces`: List all namespaces.
- `kubectl config get-contexts`: Show all contexts.
- `kubectl config use-context <context-name>`: Switch to a different context.

### 8. Others:
- `kubectl apply -f <filename>`: Apply a configuration from a file.
- `kubectl delete -f <filename>`: Delete resources defined in a file.
- `kubectl exec -it <pod-name> -- /bin/sh`: Execute a command inside a running pod.
- `kubectl port-forward <pod-name> <local-port>:<pod-port>`: Forward a port from a running pod to a local port.

### 9. Advanced:
- `kubectl get all`: List all resources.
- `kubectl rollout status deployment/<deployment-name>`: View the rollout status of a deployment.
- `kubectl rollout history deployment/<deployment-name>`: View the history of a deployment.
- `kubectl rollout undo deployment/<deployment-name>`: Rollback to a previous version of a deployment.

### 10. Monitoring & Logging:
- `kubectl top nodes`: Display resource (CPU/Memory/Storage) usage of nodes.
- `kubectl top pods`: Display resource (CPU/Memory/Storage) usage of pods.

### 11. Autoscaling:
- `kubectl autoscale deployment <deployment-name> --min=<min-pods> --max=<max-pods> --cpu-percent=<cpu-util-percentage>`: Autoscale a deployment based on CPU utilization.

### 12. Working with Helm:
- `helm list`: List releases.
- `helm install <chart>`: Install a Helm chart.
- `helm uninstall <release-name>`: Uninstall a Helm release.

### 13. Using Network Policies:
- `kubectl get networkpolicies`: List all network policies.
- `kubectl describe networkpolicy <policy-name>`: Describe a specific network policy.

### 14. Using CronJobs and Jobs:
- `kubectl get cronjobs`: List all cronjobs.
- `kubectl get jobs`: List all jobs.
- `kubectl logs job/<job-name>`: Fetch logs from a job.

### 15. Working with RBAC:
- `kubectl get roles`: List all roles in the current namespace.
- `kubectl get clusterroles`: List all cluster roles.

### 16. Using kubectl Plugins:
- `kubectl krew search`: Search plugins available for kubectl.
- `kubectl krew install <plugin-name>`: Install a kubectl plugin.

