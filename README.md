For

How to use the `curl` command be used in a Pod to retrieve all Pods in the `default` namespace? Please provide a public GitHub repository link with 1 YAML file and 1 README.md.

General outline of the process:

1.Create a ServiceAccount:
Create a ServiceAccount that will be used by the Pods to authenticate and access the Kubernetes API.

2.Create a ClusterRole and ClusterRoleBinding:
Define a ClusterRole that grants read access to Pods in the default namespace. Then, create a ClusterRoleBinding that binds the previously created ServiceAccount with the ClusterRole.

3.Create a Pod:
Create a Pod that uses the ServiceAccount created in step 1. This Pod will run the curl command to retrieve information about other Pods.

4.Run curl Command:
In the Pod's container, run the curl command against the Kubernetes API to retrieve the list of Pods in the default namespace.


