---
layout: default
title: Schema Mapped to Data.gov Equivalent
permalink: /data-dot-gov-map/
filename: data-dot-gov-map.md
published: true
---



"Common Core" Required Fields
-----------------------------

{.table .table-striped}
Field               | Definition                                                                                                                                     |JSON            | RDFa Lite  | Data.gov Equivalent  
-------             | ---------------                                                                                                                                | -------------------  | --------------  | ------- 
Title               | Human-readable name of the asset.  Should be in plain English and include sufficient detail to facilitate search and discovery.                | title           | [dct:title](http://dublincore.org/documents/2012/06/14/dcmi-terms/?v=terms#terms-title)  | Title                
Description         | Human-readable description (e.g., an abstract) with sufficient detail to enable a user to quickly understand whether the asset is of interest. | description     | [dct:description](http://dublincore.org/documents/2012/06/14/dcmi-terms/?v=terms#terms-description)  | Description          
Documentation URL   | URL to documentation for the dataset or API.  At a minimum, this should include a data dictionary and/or documentation on the API.             | dataDictionary  | [dcat:dataDictionary](http://www.w3.org/TR/vocab-dcat/#property--data-dictionary)  | Data Dictionary      
URL                 | URL to dataset or API.  This is either the direct download link for the dataset or the service endpoint for the API.                           | accessURL       | [dcat:accessURL](http://www.w3.org/TR/vocab-dcat/#property--access-download)  | Access point         
Format              | The file format or API type of the distribution                                                                                                | format          | [dcterms:format](http://www.w3.org/TR/vocab-dcat/#property--format)  | Media Format         
Tags                | Tags (or keywords) help users discover your dataset, please include terms that would be used by technical and non-technical users.             | keywords        | [dcat:keyword](http://www.w3.org/TR/vocab-dcat/#property--keyword-tag)  | Keywords             
Last Update         | Most recent date on which the dataset was changed, updated or modified.                                                                        | modified        | [dcterms:modified](http://www.w3.org/TR/vocab-dcat/#property--update-modification-date-1)  | Date updated         
Publisher           | The publishing agency.  Must use the controlled vocabulary [Coming Soon](http://vocab.data.gov) when choosing your agency name.                | organization    | [foaf:Organization](http://xmlns.com/foaf/spec/#term_Organization)  | Agency Name          
Contact Name        | Contact person's name (first, then last) for the asset                                                                                         | person           | [foaf:Person](http://xmlns.com/foaf/spec/#term_Person)  | Contact Name         
Contact Email	      | Contact person's email address			           	                                                                                               | mbox		         | [foaf:mbox](http://xmlns.com/foaf/spec/#term_mbox)  | Contact Email Address
Public              | Whether the dataset or API is available to the public (true/false)                                                                             | public          | [xsd:boolean](http://www.w3.org/TR/xmlschema-2/#boolean)  | n/a                  


"Common Core" Required if Applicable Fields
-------------------------------------------
The following fields must be used to describe each dataset if they are applicable:

{.table .table-striped}
Field               | Definition                                                                                                                                     | Data.gov Equivalent  |JSON            | RDFa Lite
-------             | ---------------                                                                                                                                | -------------------  | --------------  | ------- 
License             | The license dataset or API is published with.  See [Open Licenses](http://project-open-data.github.com/open-licenses/) for more information.   | Dataset license agreement URL | license         | [dcterms:license](http://www.w3.org/TR/vocab-dcat/#property--license-1)
Spatial  	          | The range of spatial applicability of a dataset.  Could include a spatial region like a bounding box or a named place from the [GeoNames](http://www.geonames.org) vocabulary (e.g., "Michigan").                     | Geographic scope     | spatial 	       | [dcterms:spatial](http://www.w3.org/TR/vocab-dcat/#property--spatial-geographical-coverage)
Temporal	          | The range of temporal applicability of a dataset (i.e., a start and end date of applicability for the data)                                                                                              | Period of Coverage   | temporal	       | [dcterms:temporal](http://www.w3.org/TR/vocab-dcat/#property--temporal-coverage)

Beyond Common Core -- Extending the Schema
------------------------------------------
"Extensional" and/or domain specific metadata can easily be added using other vocabularies to embedded HTML or XML markup even if it is not a term (entity/property) that will get indexed by the major search engines â€“ it could still be indexed by other custom search engines and by Data.gov.  Agencies are encouraged to extend their metadata descriptions using elements from the "Expanded Fields" list shown below, or from any well-known vocabulary (including Dublin Core, FGDC, ISO 19115, NIEM, and a growing number of vocabularies published at [vocab.data.gov](http://vocab.data.gov)) as long as they are properly assigned.

Expanded Fields
---------------
Agencies our encourage to use the following expanded fields when appropriate. Agencies may freely augment these fields with their own.

{.table .table-striped}
Field               | Definition                                                                                                                                    | Data.gov Equivalent   | JSON                  | RDFa Lite
------              | ------                                                                                                                                        | -------------------   | ----                  | --------
Release Date        | Date of formal issuance                                                                                                                       | Date Released         | issued                | [dct:issued](http://dublincore.org/documents/2012/06/14/dcmi-terms/?v=terms#issued)
Frequency           | Frequency with which dataset is published                                                                                                     | Frequency             | accrualPeriodicity    | [dct:accrualPeriodicity](http://purl.org/dc/terms/accrualPeriodicity)
Unique Identifier   | A unique identifier for the dataset or API as maintained within an Agency catalog or database                                                 | User Generated ID     | identifier            | [dcterms:identifier](http://www.w3.org/TR/vocab-dcat/#property--identifier)
Language            | The language of the dataset                                                                                                                   | n/a                   | language              | [dcat:language](http://www.w3.org/TR/vocab-dcat/#property--language-1)
Granularity         | Level of granularity of the dataset.  Typically geographical or temporal.                                                                     | Geographic Granularity  | granularity           | [dcat:granularity](http://www.w3.org/TR/vocab-dcat/#property--granularity)
Data Quality        | Describe the quality of the data                                                                                                              | Data Quality          | dataQuality           | [dcat:dataQuality](http://www.w3.org/TR/vocab-dcat/#property--data-quality)
Category            | Main thematic category of the dataset.  Could include [ISO Topic Categories](http://gcmd.nasa.gov/User/difguide/iso_topics.html)              | Subject Area          | theme                 | [dcat:theme](http://www.w3.org/TR/vocab-dcat/#property--theme-category)
Related Documents   | Related documents such as developer documentation                                                                                             | Reference for Technical Documentation | references            | [dcterms:references](http://purl.org/dc/terms/references)
Distribution        | Connects a dataset to available distributions                                                                                                 | Dataset Group Name    | distribution          | [dcat:distribution](http://www.w3.org/ns/dcat#distribution)
Size                | The size of the downloadable dataset                                                                                                          | File Size             | size                  | [dcat:size](http://www.w3.org/TR/vocab-dcat/#property--size)
Download URL        | URL providing direct access to the downloadable distribution of a dataset                                                                     | Access Point          | download              | [dcat:download](http://www.w3.org/TR/vocab-dcat/#class--download)
Homepage URL        | For presentation of results in Data.gov only: directs user to a contextual, Agency-hosted "homepage" for the Dataset or API when selecting this resource from the Data.gov user interface |n/a	| homepage	            | [foaf:homepage](http://xmlns.com/foaf/spec/#term_homepage)
Endpoint            | Endpoint of web service to access dataset                                                                                                     | Access Point          | WebService            | [dcat:webService](http://www.w3.org/TR/vocab-dcat/#class--webservice)
RSS Feed            | URL for an RSS feed that provides access to the dataset                                                                                       | Access Point          | Feed                  | [dcat:feed](http://www.w3.org/TR/vocab-dcat/#Class:_Feed)


Additional Information
----------------------
* [Schema.org](http://schema.org)
* [DCAT](http://www.w3.org/TR/vocab-dcat/)
* [vocab.data.gov](http://vocab.data.gov)


Examples (coming soon)
--------
* [JSON](examples/catalog.json)
* [XML](examples/xml/)



