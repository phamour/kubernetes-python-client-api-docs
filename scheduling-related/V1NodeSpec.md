# V1NodeSpec

NodeSpec describes the attributes that a node is created with.
## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**taints** | [**list[V1Taint]**](V1Taint.md) | If specified, the node&#39;s taints. | [optional] 
**unschedulable** | **bool** | Unschedulable controls node schedulability of new pods. By default, node is schedulable. More info: https://kubernetes.io/docs/concepts/nodes/node/#manual-node-administration | [optional] 
