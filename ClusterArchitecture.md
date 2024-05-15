https://kubernetes.io/docs/concepts/architecture/

Cluster consists of two main components:
1. **Control plane**(Master nodes)
2. **Worker Nodes**

**Control plane:**
Control plane is the one that manages the cluster and resources inside it like nodes, pods etc. The control plane is the brain behind a cluster which coordinates, schedule and maintain overall health of the cluster.

Control plane consists of multiple components in it like:

   _Kube-API Server:_ 
   Components in control plane, that exposes the K8s API, using which worker nodes able to connect and communicate with control plane

   _etcd:_
   etcd stores all cluster data(operational data) and ensures backup. etcd is a highly available key value store used for data storage and data backup.

   _kube-scheduler:_
   Component that select a available node to run a pod on. When ever there is new pod created kube-scheduler will looks for available node with available resources, affinity, anti-affinity specifications etc and schedule a pod to run on a correct node.

   
