# V1WeightedPodAffinityTerm

The weights of all of the matched WeightedPodAffinityTerm fields are added per-node to find the most preferred node(s)
## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**pod_affinity_term** | [**V1PodAffinityTerm**](V1PodAffinityTerm.md) |  | 
**weight** | **int** | weight associated with matching the corresponding podAffinityTerm, in the range 1-100. | 
