# Microservices-setup

## Accessing a Cluster Using kubectl
kubectl is a command-line tool provided by Kubernetes, enabling you to manage cluster resources, view cluster status, deploy applications, and debug issues through the CLI, you can click on this [link](https://support.huaweicloud.com/intl/en-us/usermanual-cce/cce_10_0107.html#section0) to access the official docs for using kubectl and getting the kubeconfig file. kubectl retrieves cluster information from a kubeconfig file and communicates with the Kubernetes API server. The kubeconfig file is the identity credential for kubectl to access the Kubernetes cluster. It contains the API server address, user authentication credentials, and other configuration details. With these details, kubectl can interact with the Kubernetes cluster to perform management tasks.

### Prerequisites
- A client computer that can access the Internet is available.
- Before using intranet access, ensure that the client and the cluster to be accessed are in the same VPC.

  Typically you would be using intranet access, so when obtaining the kubeconfig file, in the kubeconfig file area, select Private access as shown below 
  <img width="990" height="553" alt="image" src="https://github.com/user-attachments/assets/0de0204c-2269-4ca4-b98b-55b24d58a10a" />


Follow the instructions docs in this [link](https://support.huaweicloud.com/intl/en-us/usermanual-cce/cce_10_0107.html#section6) to install kubectl on the client.

To use a Permanent alias `k` (so it works every time you open a shell instead of using `kubectl`)
Add the alias to your shell config file (~/.bashrc, ~/.zshrc, etc.):
```
echo "alias k=kubectl" >> ~/.bashrc
source ~/.bashrc
```
