# V1PodSpec

PodSpec is a description of a pod.
## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**affinity** | [**V1Affinity**](V1Affinity.md) |  | [optional] 
**containers** | [**list[V1Container]**](V1Container.md) | List of containers belonging to the pod. Containers cannot currently be added or removed. There must be at least one container in a Pod. Cannot be updated. | 
**node_selector** | **dict(str, str)** | NodeSelector is a selector which must be true for the pod to fit on a node. Selector which must match a node&#39;s labels for the pod to be scheduled on that node. More info: https://kubernetes.io/docs/concepts/configuration/assign-pod-node/ | [optional] 
**preemption_policy** | **str** | PreemptionPolicy is the Policy for preempting pods with lower priority. One of Never, PreemptLowerPriority. Defaults to PreemptLowerPriority if unset. This field is beta-level, gated by the NonPreemptingPriority feature-gate. | [optional] 
**priority** | **int** | The priority value. Various system components use this field to find the priority of the pod. When Priority Admission Controller is enabled, it prevents users from setting this field. The admission controller populates this field from PriorityClassName. The higher the value, the higher the priority. | [optional] 
**priority_class_name** | **str** | If specified, indicates the pod&#39;s priority. \&quot;system-node-critical\&quot; and \&quot;system-cluster-critical\&quot; are two special keywords which indicate the highest priorities with the former being the highest priority. Any other name must be defined by creating a PriorityClass object with that name. If not specified, the pod priority will be default or zero if there is no default. | [optional] 
**scheduler_name** | **str** | If specified, the pod will be dispatched by specified scheduler. If not specified, the pod will be dispatched by default scheduler. | [optional] 
**tolerations** | [**list[V1Toleration]**](V1Toleration.md) | If specified, the pod&#39;s tolerations. | [optional] 
**topology_spread_constraints** | [**list[V1TopologySpreadConstraint]**](V1TopologySpreadConstraint.md) | TopologySpreadConstraints describes how a group of pods ought to spread across topology domains. Scheduler will schedule pods in a way which abides by the constraints. All topologySpreadConstraints are ANDed. | [optional] 
