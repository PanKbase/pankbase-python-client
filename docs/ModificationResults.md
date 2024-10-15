# ModificationResults


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**graph** | [**List[Modification]**](Modification.md) |  | [optional] 
**id** | **str** |  | [optional] 
**type** | **List[str]** |  | [optional] 
**total** | **int** |  | [optional] 
**facets** | [**List[SearchFacet]**](SearchFacet.md) |  | [optional] 

## Example

```python
from igvf_client.models.modification_results import ModificationResults

# TODO update the JSON string below
json = "{}"
# create an instance of ModificationResults from a JSON string
modification_results_instance = ModificationResults.from_json(json)
# print the JSON string representation of the object
print(ModificationResults.to_json())

# convert the object into a dict
modification_results_dict = modification_results_instance.to_dict()
# create an instance of ModificationResults from a dict
modification_results_from_dict = ModificationResults.from_dict(modification_results_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


