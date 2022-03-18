# V1NodeStatus

NodeStatus is information about the current status of a node.
## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**addresses** | [**list[V1NodeAddress]**](V1NodeAddress.md) | List of addresses reachable to the node. Queried from cloud provider, if available. More info: https://kubernetes.io/docs/concepts/nodes/node/#addresses Note: This field is declared as mergeable, but the merge key is not sufficiently unique, which can cause data corruption when it is merged. Callers should instead use a full-replacement patch. See http://pr.k8s.io/79391 for an example. | [optional] 
**allocatable** | **dict(str, str)** | Allocatable represents the resources of a node that are available for scheduling. Defaults to Capacity. | [optional] 
**capacity** | **dict(str, str)** | Capacity represents the total resources of a node. More info: https://kubernetes.io/docs/concepts/storage/persistent-volumes#capacity | [optional] 
**conditions** | [**list[V1NodeCondition]**](V1NodeCondition.md) | Conditions is an array of current observed node conditions. More info: https://kubernetes.io/docs/concepts/nodes/node/#condition | [optional] 
**images** | [**list[V1ContainerImage]**](V1ContainerImage.md) | List of container images on this node | [optional] 
**node_info** | [**V1NodeSystemInfo**](V1NodeSystemInfo.md) |  | [optional] 
