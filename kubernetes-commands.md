Here’s a structured guide for Kubernetes commands:

# Kubernetes Command Reference Guide

A comprehensive guide to essential Kubernetes commands for managing and deploying containerized applications.

---

## Kubernetes Basics
1. **`kubectl version`**: Displays the version of Kubernetes client and server.
2. **`kubectl cluster-info`**: Shows information about the Kubernetes cluster, including the API server's address.
3. **`kubectl get nodes`**: Lists all nodes in the cluster.
4. **`kubectl describe node <node_name>`**: Provides detailed information about a specific node.

---

## Managing Pods
5. **`kubectl get pods`**: Lists all pods in the current namespace.
6. **`kubectl get pods -n <namespace>`**: Lists all pods in a specified namespace.
7. **`kubectl describe pod <pod_name>`**: Shows detailed information about a specific pod.
8. **`kubectl logs <pod_name>`**: Displays logs from a specific pod.
9. **`kubectl exec -it <pod_name> -- <command>`**: Executes a command inside a running pod (e.g., starting a bash shell).
10. **`kubectl delete pod <pod_name>`**: Deletes a specific pod.

---

## Working with Deployments
11. **`kubectl get deployments`**: Lists all deployments in the current namespace.
12. **`kubectl describe deployment <deployment_name>`**: Shows detailed information about a specific deployment.
13. **`kubectl create deployment <deployment_name> --image=<image_name>`**: Creates a deployment using a specified image.
14. **`kubectl scale deployment <deployment_name> --replicas=<number>`**: Scales a deployment to the specified number of replicas.
15. **`kubectl rollout restart deployment <deployment_name>`**: Restarts a deployment to apply updated configurations.
16. **`kubectl delete deployment <deployment_name>`**: Deletes a specific deployment.

---

## Services and Networking
17. **`kubectl get services`**: Lists all services in the current namespace.
18. **`kubectl describe service <service_name>`**: Provides detailed information about a specific service.
19. **`kubectl expose deployment <deployment_name> --type=<service_type> --port=<port>`**: Creates a service for a deployment.
20. **`kubectl port-forward <pod_name> <host_port>:<pod_port>`**: Forwards a local port to a pod.

---

## Namespaces
21. **`kubectl get namespaces`**: Lists all namespaces in the cluster.
22. **`kubectl create namespace <namespace_name>`**: Creates a new namespace.
23. **`kubectl delete namespace <namespace_name>`**: Deletes a specified namespace.
24. **`kubectl config set-context --current --namespace=<namespace_name>`**: Sets a default namespace for the current context.

---

## ConfigMaps and Secrets
25. **`kubectl create configmap <config_name> --from-literal=<key>=<value>`**: Creates a ConfigMap from literal values.
26. **`kubectl describe configmap <config_name>`**: Displays details of a specific ConfigMap.
27. **`kubectl delete configmap <config_name>`**: Deletes a specific ConfigMap.
28. **`kubectl create secret generic <secret_name> --from-literal=<key>=<value>`**: Creates a secret from literal values.
29. **`kubectl describe secret <secret_name>`**: Provides detailed information about a specific secret.

---

## Managing Resources
30. **`kubectl apply -f <file_name>`**: Applies changes from a configuration file.
31. **`kubectl delete -f <file_name>`**: Deletes resources defined in a configuration file.
32. **`kubectl get all`**: Lists all resources in the current namespace, including pods, services, and deployments.

---

## Debugging and Troubleshooting
33. **`kubectl describe <resource_type> <resource_name>`**: Displays detailed information about a resource (e.g., pod, service, deployment).
34. **`kubectl top pod`**: Shows resource usage of pods.
35. **`kubectl top node`**: Displays resource usage of nodes.
36. **`kubectl events`**: Streams real-time events from the cluster.
37. **`kubectl exec -it <pod_name> -- <command>`**: Access a container in a pod to debug issues.

---

## Advanced Operations
38. **`kubectl rollout status deployment <deployment_name>`**: Checks the status of a deployment rollout.
39. **`kubectl set image deployment/<deployment_name> <container_name>=<new_image>`**: Updates the image of a deployment's container.
40. **`kubectl cordon <node_name>`**: Marks a node as unschedulable.
41. **`kubectl drain <node_name>`**: Safely evicts all pods from a node.
42. **`kubectl taint nodes <node_name> <key>=<value>:<effect>`**: Applies a taint to a node to control pod scheduling.

---

This guide covers the most commonly used Kubernetes commands to help you manage and deploy containerized applications efficiently. Bookmark this for quick reference!
