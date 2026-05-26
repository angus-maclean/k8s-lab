
# What is a Service in Kubernetes?

- When pods die and are replaced, they get a new IP address
- If users or other pods were connected to the pod then communication is lost

- When you make a service you give pods a stable IP address that stays
- We just made a NodePort service type. There are ClusterIP and LoadBalancer service types too



# THREE SERVICE TYPES

## NodePort

Allows pods to talk to each other WITHIN a cluster.


## ClusterIP

Allows external users to access pods inside the cluster.

## Load Balancer

A production level ClusterIP. 







# Basic networking with a service

Pod
- has a TARGET PORT

Service
- has a PORT

Node
- has a NODE PORT


The TARGET PORT on the Pod, and PORT on the Service are the same and are mapped to eachother. 

The NODE PORT is connected to the Service.

## Flow of traffic

External traffic -> node: NODE PORT -> service: PORT -> pod:TARGET PORT


#Load Balancer - Service Type

