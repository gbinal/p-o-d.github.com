---
layout: default
title: Metadata Resources
permalink: /metadata-resources/
filename: metadata-resources.md
published: false
---

<table width="60%">
<b><tr><td><ul>
<li><a href="#template_data_files">Template Data Files</a></li>
<li><a href="#sample_data_files">Sample Data Files</a></li>
<li><a href="#metadata_field_guidance">Schema Guidance</a></li>
</ul></td>
<td><ul>
<li><a href="#schema_maps">Schema Maps</a></li>
<li><a href="#use_cases">Use Cases</a></li>
<li><a href="#faq">FAQ</a></li>
</ul></td></tr></b>
</table>
-------------------

### Template Data Files
* [CSV]()
* [JSON]()
* [XML]()
* [RDFa Lite]()


### Sample Data Files
* [CSV]()
* [JSON]()
* [XML]()
* [RDFa Lite]()

### Metadata Field  Guidance

catalogs/norms for each item in schema... (Under construction)

### Schema Maps

A breakdown of the data.json schema as [mapped to other related schemas]().  

### Use Cases  
  
A) Starting from a spreadsheet

Some agencies may initially build or maintain data catalogs through large spreadsheets.  In order to then generate a data.json file from this, simply import the spreadsheet (in the form of a .csv) into the [Catalog Generator](http://project-open-data.github.com/catalog-generator/), translate the metadata as needed, and then generate an appropriately formatted .json file.  

B) Translating a data file from another schema

If your agency has a .json catalog with a different metadata schema and need to convert it to the prescribed schema needed for the data.json file, one can import the file into [Catalog Generator](http://project-open-data.github.com/catalog-generator/), adjust the metadata as needed and export the results again as the appropriately formatted .json file.  

C) Utilizing CKAN 

[CKAN](http://www.CKAN.org) is a popular, open-source data catalog.  Even if an agency hasn't begun a data catalog, adopting CKAN can provide a robust and feature-rich solution with which to begin maintaining an internal or external catalog.  In addition to providing an effective means of organizing the agency's data catalog, CKAN provides several opportunities for generating the needed data.json file.  CKAN provides a convenient .csv export that can then be imported into the [Catalog Generator](http://project-open-data.github.com/catalog-generator/) for conversion into an appropriately formatted .json file.  Alternatively, CKAN provides a JSON API of the data catalog which can then be altered to provide an automatic update for the appropriately formatted .json file.  

D) Manual translating a data file from another system

Agencies may also manage their data catalogs through various database solutions such as Access, an asset management sytem, document management system, geoportal or assorted proprietary systems.  Regardless of which system an agency employs, it should include a fundamental export option which allows the catalog to be exported as a .csv, which can then be imported into the [Catalog Generator](http://project-open-data.github.com/catalog-generator/) for conversation to an appropriately formatted .json file.  Depending on the solutions' varied further functionality, some of them may also provide APIs which can then be configured to maintain the data.json file.  If not, they may instead support an .xml and .json exports which can then be converted to the proper format.


### FAQ

