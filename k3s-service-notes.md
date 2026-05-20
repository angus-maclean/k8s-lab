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
