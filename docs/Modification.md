# Modification

A genetic modification altering sample genomic material. For example, CRISPRi dCas9-KRAB modification.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**release_timestamp** | **str** | The date the object was released. | [optional] 
**sources** | **List[str]** | The originating lab(s) or vendor(s). | [optional] 
**lot_id** | **str** | The lot identifier provided by the originating lab or vendor. | [optional] 
**product_id** | **str** | The product or catalog identifier provided following deposition to addgene.org. | [optional] 
**documents** | **List[str]** | Documents that provide additional information (not data file). | [optional] 
**status** | **str** | The status of the metadata object. | [optional] 
**lab** | **str** | Lab associated with the submission. | [optional] 
**award** | **str** | Grant associated with the submission. | [optional] 
**schema_version** | **str** | The version of the JSON schema that the server uses to validate the object. | [optional] 
**uuid** | **str** | The unique identifier associated with every object. | [optional] 
**notes** | **str** | DACC internal notes. | [optional] 
**aliases** | **List[str]** | Lab specific identifiers to reference an object. | [optional] 
**creation_timestamp** | **str** | The date the object was created. | [optional] 
**submitted_by** | **str** | The user who submitted the object. | [optional] 
**submitter_comment** | **str** | Additional information specified by the submitter to be displayed as a comment on the portal. | [optional] 
**description** | **str** | A plain text description of the object. | [optional] 
**cas** | **str** | The name of the CRISPR associated protein used in the modification. | [optional] 
**fused_domain** | **str** | The name of the molecule fused to a Cas protein. | [optional] 
**modality** | **str** | The purpose or intended effect of a CRISPR modification. | [optional] 
**tagged_protein** | **str** | The tagged protein in modifications in which the Cas nuclease is fused to an antibody. | [optional] 
**cas_species** | **str** | The originating species of the Cas nuclease. | [optional] 
**activated** | **bool** | A boolean indicating whether the modification has been activated by a chemical agent. | [optional] 
**activating_agent_term_id** | **str** | The CHEBI identifier for the activating agent of the modification. | [optional] 
**activating_agent_term_name** | **str** | The CHEBI name for the activating agent of the modification. | [optional] 
**id** | **str** |  | [optional] 
**type** | **List[str]** |  | [optional] 
**summary** | **str** |  | [optional] 
**biosamples_modified** | **List[str]** | The biosamples which have been modified with this modification. | [optional] 

## Example

```python
from igvf_client.models.modification import Modification

# TODO update the JSON string below
json = "{}"
# create an instance of Modification from a JSON string
modification_instance = Modification.from_json(json)
# print the JSON string representation of the object
print(Modification.to_json())

# convert the object into a dict
modification_dict = modification_instance.to_dict()
# create an instance of Modification from a dict
modification_from_dict = Modification.from_dict(modification_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


