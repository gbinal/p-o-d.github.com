---
layout: default
title: Common Core Metadata Schema
permalink: /schema/
filename: schema.md
published: true
---

This repository contains guidance to support the use of standard metadata schema to list agency datasets and Application Programming Interfaces (APIs) as hosted at agency.gov/data.  

Standard Metadata Vocabulary
----------------------------
Metadata are selected fields or elements which describe data. The challenge is to define the standard metadata fields and the names of those fields so that the consumer of the data has sufficient information to process and understand the data. The more information that can be conveyed in a standardized regular format, the more valuable data becomes. Metadata can range from basic to advanced, from allowing one to discover the mere fact that a certain data asset exists and is about a general subject all the way to providing detailed semantic information that enables a high degree of machine readability. Making the metadata machine readable greatly increases its openness and utility.

Establishing a common vocabulary is the key to any communication, including communication between machines.  [Schema.org](http://www.schema.org) is a hierarchical vocabulary that is being developed through a collaboration of the major search engines and serves as the basis for the **common core metadata** required in this memorandum. The standard consists of a number of schemas (hierarchical vocabulary terms) that represent things that are most often looked for on the web and encapsulates many of the early lessons learned from vocabulary development.  


What to Document -- Datasets and APIs
-------------------------------------

APIs allow developers (both internal to the agency and the public) to dynamically query a dataset. For example, a dataset [of farmers markets](https://explore.data.gov/Agriculture/Farmers-Markets-Geographic-Data/wfna-38ey) may be made available for download as a single file (e.g., a CSV), or may be made available to developers as an API, such that a developer could provide the agency with a zipcode, and retrieve a list of farmers markets in that area.

The catalog file should list all of an agencies datasets that can be made public, regardless of form - this includes raw datasets and APIs.  Use **webService** to indicate which datasets offer dynamic APIs (see below for more information on Common Core and Extensional metadata elements).


Metadata File Formats --  RDFa and JSON
---------------------------------------
The [Implemention Guidance](http://gsa-ocsit.github.com/project-open-data.github.com//implementation-guide/) available as a part of Project Open Data describes Agency requirements for the development of metadata as per the Open Data Policy.  A quick primer on the two file formats involved:

[JSON](http://www.json.org) is a lightweight data-exchange format that is very easy to read, parse and generate.  Based on a subset of the JavaScript programming language, JSON is a text format that is optimized for data interchange.  JSON is built on two structures: (1) a collection of name/value pairs; and (2) an ordered list of values.  

[RDFa Lite](http://www.w3.org/TR/rdfa-lite/) is a minimal subset of RDFa, the Resource Description Framework in attributes, consisting of a few attributes that may be used to express machine-readable data in Web documents like HTML and XML. While it is not a complete solution for advanced data markup tasks, it allows users to publish metadata in a way that is immediately understandable by search engines and other applications built to leverage the growing "web of data."  

Links to downloadable examples of metadata files developed in these and other formats in [the metadata resources](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/).  Tools to help agencies produce and maintain their data inventories are [available on GitHub](http://www.github.com/project-open-data) and hosted at [Labs.Data.gov](http://labs.data.gov).


"Common Core" Required Fields
-----------------------------
The following "common core" fields are required, to be used to describe each entry:

(*Select the links in RDFa Lite column to learn more about the use of each element, including the range of valid entries where appropriate. [Consult the schema maps to find the equivalent Data.gov fields](http://gsa-ocsit.github.com/project-open-data.github.com/data-dot-gov-map/).*)

{.table .table-striped}
Field               | Definition                                                                                                                                     |JSON            
-------             | ---------------                                                                                                                                | --------------  
Title               | Human-readable name of the asset.  Should be in plain English and include sufficient detail to facilitate search and discovery. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                | title           
Description         | Human-readable description (e.g., an abstract) with sufficient detail to enable a user to quickly understand whether the asset is of interest. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps)) | description     
Download URL        | URL providing direct access to the downloadable distribution of a dataset. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                                                                     | download              
Format              | The file format or API type of the distribution. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                                                                                                | format          
Tags                | Tags (or keywords) help users discover your dataset, please include terms that would be used by technical and non-technical users. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))             | keywords        
Last Update         | Most recent date on which the dataset was changed, updated or modified. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                                                                        | modified        
Publisher           | The publishing agency. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                | organization    
Contact Name      | Contact person's name for the asset. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                                                                                       | person         
Contact Email	    | Contact person's email address. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))			           	                                                                             | mbox	       
Unique Identifier   | A unique identifier for the dataset or API as maintained within an Agency catalog or database. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                                                 | identifier            
Public Access Level | The degree to which this dataset **could** be made publicly-available, *regardless of whether it has been made available*. Choices: Public (is or *could be* made publicly available), Restricted (available under certain conditions), Private (never able to be made publicly available) ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps)) | access          

"Common Core" Required if Applicable Fields
-------------------------------------------
The following fields must be used to describe each dataset if they are applicable:

{.table .table-striped}
Field               | Definition                                                                                                                                     |JSON            
-------             | ---------------                                                                                                                                | --------------  
Documentation URL   | URL to documentation for the dataset or API.  At a minimum, this should include a data dictionary and/or documentation on the API. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))             | dataDictionary  
Endpoint            | Endpoint of web service to access dataset. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                                                                                                     | webService            
License             | The license dataset or API is published with.  See [Open Licenses](http://gsa-ocsit.github.com/project-open-data.github.com/open-licenses/) for more information. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))   | license         
Spatial  	    | The range of spatial applicability of a dataset.  Could include a spatial region like a bounding box or a named place. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                     | spatial 	       
Temporal	    | The range of temporal applicability of a dataset (i.e., a start and end date of applicability for the data). ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                                    | temporal	       

Beyond Common Core -- Extending the Schema
------------------------------------------
"Extensional" and/or domain specific metadata can easily be added using other vocabularies to embedded HTML or XML markup even if it is not a term (entity/property) that will get indexed by the major search engines - it could still be indexed by other custom search engines and by Data.gov.  Agencies are encouraged to extend their metadata descriptions using elements from the "Expanded Fields" list shown below, or from any well-known vocabulary (including Dublin Core, FGDC, ISO 19115, NIEM, and a growing number of vocabularies published at [vocab.data.gov](http://vocab.data.gov)) as long as they are properly assigned.

Expanded Fields
---------------
Agencies are encouraged to use the following expanded fields when appropriate. Agencies may freely augment these fields with their own.

{.table .table-striped}
Field               | Definition                                                                                                                                    | JSON                 
------              | ------                                                                                                                                        | ----                  
Release Date        | Date of formal issuance. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                                                                                                                       | issued         
Frequency           | Frequency with which dataset is published. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                                                                                                     | accrualPeriodicity    
Language            | The language of the dataset. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                                                                                                                   | language              
Granularity         | Level of granularity of the dataset.  Typically geographical or temporal. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                                                                     | granularity           
Data Quality        | Whether the dataset meets the agency's Information Quality Guidelines (true/false). ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                                                                                                              | dataQuality          
Category            | Main thematic category of the dataset. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))               | theme                 
Related Documents   | Related documents such as developer documentation. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                                                                                             | references            
Distribution        | Connects a dataset to available distributions. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                                                                                                 | distribution         
Size                | The size of the downloadable dataset. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                                                                                                          | size                  
Homepage URL        | Alternative landing page used to redirect user to a contextual, Agency-hosted "homepage" for the Dataset or API when selecting this resource from the Data.gov user interface. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps)) | homepage	            
RSS Feed            | URL for an RSS feed that provides access to the dataset. ([?](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/#schema_maps))                                                                                       | feed                 


Additional Information
----------------------
* [Schema.org](http://schema.org)
* [DCAT](http://www.w3.org/TR/vocab-dcat/)
* [vocab.data.gov](http://vocab.data.gov)


Examples
--------
* [JSON](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/)
* [RDFa Lite](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/)
* [XML](http://gsa-ocsit.github.com/project-open-data.github.com/metadata-resources/)
