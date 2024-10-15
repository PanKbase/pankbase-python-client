# HumanDonor

A human donor of any biosample, including cell lines. Submission of any sample originating from a human donor requires submission of information about the relevant donor. For example, submission of the donor of K562 is a prerequisite for submission of any K562 cell line samples. The following fields are **required**: `award`, `lab`, `rrid`, `living_donor`, `bmi`, `diabetes_status`, `diabetes_status_description`, and `taxa`. These fields must be included for the schema to be valid. Additionally, the following fields are **desired**: `center_donor_id`, `ethnicities`, `hba1c`, `diabetes_status_hba1c`, `glucose_loweing_theraphy`, `hospital_stay`, `donation_type`, and `cause_of_death`. While these fields are not mandatory, their inclusion is highly recommended for a more comprehensive data submission.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**release_timestamp** | **str** | The date the object was released. | [optional] 
**taxa** | **str** | The species of the organism. | [optional] 
**publication_identifiers** | **List[str]** | The publication identifiers that provide more information about the object. | [optional] 
**url** | **str** | An external resource with additional information. | [optional] 
**documents** | **List[str]** | Documents that provide additional information (not data file). | [optional] 
**lab** | **str** | Lab associated with the submission. | [optional] 
**award** | **str** | Grant associated with the submission. | [optional] 
**accession** | **str** | A unique identifier to be used to reference the object prefixed with PKB. | [optional] 
**alternate_accessions** | **List[str]** | Accessions previously assigned to objects that have been merged with this object. | [optional] 
**collections** | **List[str]** | Some samples are part of particular data collections. | [optional] 
**status** | **str** | The status of the metadata object. | [optional] 
**revoke_detail** | **str** | Explanation of why an object was transitioned to the revoked status. | [optional] 
**schema_version** | **str** | The version of the JSON schema that the server uses to validate the object. | [optional] 
**uuid** | **str** | The unique identifier associated with every object. | [optional] 
**notes** | **str** | DACC internal notes. | [optional] 
**aliases** | **List[str]** | Lab specific identifiers to reference an object. | [optional] 
**creation_timestamp** | **str** | The date the object was created. | [optional] 
**submitted_by** | **str** | The user who submitted the object. | [optional] 
**submitter_comment** | **str** | Additional information specified by the submitter to be displayed as a comment on the portal. | [optional] 
**description** | **str** | A plain text description of the object. | [optional] 
**dbxrefs** | **List[str]** | Identifiers from external resources that may have 1-to-1 or 1-to-many relationships with IGVF donors. | [optional] 
**sex** | **str** | Self-Reported sex of the donor. | [optional] 
**phenotypic_features** | **List[str]** | A list of associated phenotypic features of the donor. | [optional] 
**virtual** | **bool** | Virtual donors are not representing actual human or model organism donors, samples coming from which were used in experiments, but rather capturing metadata about hypothetical donors that the reported analysis results are relevant for. | [optional] 
**ethnicities** | **List[str]** | Self-Reported Ethnicity of the donor. | [optional] 
**genetic_ethnicities** | **List[str]** | Inferred ancestry of the donor from genetic analysis | [optional] 
**living_donor** | **bool** | Living Donor | [optional] 
**family_history_of_diabetes** | **str** | Family History of Diabetes | [optional] 
**family_history_of_diabetes_relationship** | **List[str]** | Family History of Diabetes Relationship. | [optional] 
**rrid** | **str** | Research Unique Identifier. PanKbase will only take donors with RRID | [optional] 
**pancreas_tissue_available** | **bool** | Pancreas tissue is available for research or analysis | [optional] 
**center_donor_id** | **str** | Donor center ID identifier for cross-referencing | [optional] 
**biological_sex** | **str** | Inferred biological sex derived from genomic data | [optional] 
**age** | **float** | Age in years | [optional] 
**bmi** | **float** | Body mass index (Kg/m2) | [optional] 
**diabetes_duration** | **str** | Diabetes Duration in years | [optional] 
**diabetes_status** | **List[str]** | Diabetes status T1D,T2D,MODY, etc. MONDO ontology term | [optional] 
**diabetes_status_description** | **str** | Description of diabetes status | [optional] 
**hba1c** | **float** | The percentage measurement of HbA1c, which reflects the average blood glucose levels over the past 2-3 months.  If not available, &#39;NA&#39; | [optional] 
**diabetes_status_hba1c** | **str** | A categorization of diabetes status based on adjusted HbA1C levels, considering factors such as age, race, or other clinical conditions that might influence HbA1C measurements | [optional] 
**donation_type** | **str** | The type of organ donation, categorized as DCD, NDD, or MAID | [optional] 
**cause_of_death** | **str** | The primary medical condition or event that led to the patient’s death | [optional] 
**c_peptide** | **float** | The concentration of C-Peptide in the blood, a marker used to assess insulin production and pancreatic function | [optional] 
**aab_gada** | **bool** | The presence of Autoantibodies against GADA | [optional] 
**aab_gada_value** | **float** | AAB GADA value (unit/ml) | [optional] 
**aab_ia2** | **bool** | The presence of Autoantibodies against IA2 | [optional] 
**aab_ia2_value** | **float** | AAB IA2 value (unit/ml) | [optional] 
**aab_znt8** | **bool** | The presence of Autoantibodies against ZNT8 | [optional] 
**aab_znt8_value** | **float** | AAB ZNT8 value (unit/ml) | [optional] 
**hla_typing** | **List[str]** | Series of comma-separated values describing HLA types as: class, locus, allele1, allele2, method | [optional] 
**other_tissues_available** | **List[str]** | Tissues obtained from the donor | [optional] 
**hospital_stay** | **float** | The total number of days the patient was hospitalized | [optional] 
**glucose_loweing_theraphy** | **List[str]** | Details the type of therapy or medication regimen the patient is on to manage blood glucose levels, including oral medications, insulin, or other treatments. | [optional] 
**human_donor_identifiers** | **List[str]** | Identifiers of this human donor. | [optional] 
**id** | **str** |  | [optional] 
**type** | **List[str]** |  | [optional] 
**summary** | **str** | A summary of the human donor. | [optional] 

## Example

```python
from igvf_client.models.human_donor import HumanDonor

# TODO update the JSON string below
json = "{}"
# create an instance of HumanDonor from a JSON string
human_donor_instance = HumanDonor.from_json(json)
# print the JSON string representation of the object
print(HumanDonor.to_json())

# convert the object into a dict
human_donor_dict = human_donor_instance.to_dict()
# create an instance of HumanDonor from a dict
human_donor_from_dict = HumanDonor.from_dict(human_donor_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


