# object-model

TOPIC : ks8 Object Model

Five types of objects model :
1. Namespace (imp)
2. POD
3. Replicase
4. Deployment
5. Service

1. Namespace : In computing, a namespace is a set of signs (names) that are used to identify and refer to objects of various kinds.
namespace is like a package name , logical partitioning in kubernatives cluster is said to be namespace.

In Kubernetes, namespaces provides a mechanism for isolating groups of resources within a single cluster. Names of resources need to be unique within a namespace, but not across namespaces. Namespace-based scoping is applicable only for namespaced objects (e.g. Deployments, Services, etc) and not for cluster-wide objects (e.g. StorageClass, Nodes, PersistentVolumes, etc).

2. POD – Pod is a collection of one or more containers that share storage and network resources. Pods contain the definition of how the containers should be run in Minikube. Minikube uses these definitions to maintain the necessary resources. For example, you can define you need two pods.

During execution, if a pod goes down, Minikube will automatically fire up a new pod.

3. ReplicaSet : A ReplicaSet (RS) is a Kubernetes object that ensures there is always a stable set of running pods for a specific workload. The ReplicaSet configuration defines a number of identical pods required, and if a pod is evicted or fails, creates more pods to compensate for the loss.

4. Deployments : A Deployment provides declarative updates for Pods and ReplicaSets.
You describe a desired state in a Deployment, and the Deployment Controller changes the actual state to the desired state at a controlled rate. You can define Deployments to create new ReplicaSets, or to remove existing Deployments and adopt all their resources with new Deployments.

