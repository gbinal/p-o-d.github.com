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

</ul></td></tr></b>
</table>
-------------------

### Template Data Files

<table width="60%">
<b><tr><td><ul>
<li><a href="https://raw.github.com/GSA-OCSIT/project-open-data.github.com/gh-pages/assets/catalog-template.json">JSON</a></li>
<li><a href="https://raw.github.com/GSA-OCSIT/project-open-data.github.com/gh-pages/assets/catalog-template.xml">XML</a></li>
<li><a href="https://raw.github.com/GSA-OCSIT/project-open-data.github.com/gh-pages/assets/catalog-template.html">RDFa Lite</a></li>
<li><a href="https://raw.github.com/GSA-OCSIT/project-open-data.github.com/gh-pages/assets/catalog-template.csv">CSV</a></li>
</ul></td>
<td><ul>
<li><a href="https://raw.github.com/GSA-OCSIT/project-open-data.github.com/gh-pages/assets/catalog-template-extended.json">JSON (Extended)</a></li>
<li><a href="https://raw.github.com/GSA-OCSIT/project-open-data.github.com/gh-pages/assets/catalog-template-extended.xml">XML (Extended)</a></li>
<li><a href="https://raw.github.com/GSA-OCSIT/project-open-data.github.com/gh-pages/assets/catalog-template-extended.html">RDFa Lite (Extended)</a></li>
<li><a href="https://raw.github.com/GSA-OCSIT/project-open-data.github.com/gh-pages/assets/catalog-template-extended.csv">CSV (Extended)</a></li>
</ul></td></tr></b>
</table>

### Sample Data Files

<table width="60%">
<b><tr><td><ul>
<li><a href="https://raw.github.com/GSA-OCSIT/project-open-data.github.com/gh-pages/assets/catalog-sample.json">JSON</a></li>
<li><a href="https://raw.github.com/GSA-OCSIT/project-open-data.github.com/gh-pages/assets/catalog-sample.xml">XML</a></li>
<li><a href="https://raw.github.com/GSA-OCSIT/project-open-data.github.com/gh-pages/assets/catalog-sample.html">RDFa Lite</a></li>
<li><a href="https://raw.github.com/GSA-OCSIT/project-open-data.github.com/gh-pages/assets/catalog-sample.csv">CSV</a></li>
</ul></td>
<td><ul>
<li><a href="https://raw.github.com/GSA-OCSIT/project-open-data.github.com/gh-pages/assets/catalog-sample-extended.json">JSON (Extended)</a></li>
<li><a href="https://raw.github.com/GSA-OCSIT/project-open-data.github.com/gh-pages/assets/catalog-sample-extended.xml">XML (Extended)</a></li>
<li><a href="https://raw.github.com/GSA-OCSIT/project-open-data.github.com/gh-pages/assets/catalog-sample-extended.html">RDFa Lite (Extended)</a></li>
<li><a href="https://raw.github.com/GSA-OCSIT/project-open-data.github.com/gh-pages/assets/catalog-sample-extended.csv">CSV (Extended)</a></li>
</ul></td></tr></b>
</table>

### Schema Maps

A breakdown of the data.json schema as [mapped to its pre-existing Data.gov equivalent](data-dot-gov-map).

### Further Metadata Field Guidance

**Title**  
Acronyms should be avoided.  

Cardinality: (1,1)  

**Description**  

Cardinality: (1,1)  

**Documentation URL**  

Cardinality: (1,1)  

**Download URL**  

Cardinality: (1,n)  

**Format**  
Express this field using file extensions (e.g., CSV, XLS, XLSX, TSV, JSON, XML).  Separate multiple entries with commas or by using the Distribution field (see below).  

Cardinality: (1,n)  

**Tags**  
Should be separated by commas.  

Cardinality: (1,n)  

**Last Update**  
Dates should be formatted as MM/DD/YYYY.  

Cardinality: (1,1)  

**Publisher**  
Departments and multi-unit agencies may use this field to describe which subordinate agency published this dataset.  

Cardinality: (1,1)  


**Contact Name**  

Name should be formatted as Last, First. 

Cardinality: (1,1)  


**Contact Email**  

Cardinality: (1,1)  

**Unique Identifier**  
This field allows third parties to maintain a consistent record for datasets even if title or urls are updated.  Agencies may integrate an existing system for maintaining unique identifiers or enter arbitrary characters for this field, however the fundamental requirement be that each identifier be unique across the agency's data catalog and remain fixed to the dataset.  Characters should be alphanumeric.  

Cardinality: (1,1)  

**Public**  


Cardinality: (1,1)  

**Endpoint**    
This field will serve to delineate the web services offered by an agency and will be used to aggregate cross-government API catalogs.  It must be included for each public API offered by the agency.  

Cardinality: (0,1)  

**License**  

Cardinality: (0,1)  

**Spatial**  

Cardinality: (0,1)  

**Temporal**  

Cardinality: (0,1)  



**Release Date**  
Dates should be formatted as MM/DD/YYYY.  

Cardinality: (0,1)  

**Frequency**  
Frequency should be one of the following: hourly, daily, weekly, yearly, other. 

Cardinality: (0,1)  

**Language**  

Cardinality: (0,n)  

**Granularity**  

Cardinality: (0,1)  

**Data Quality**  


Cardinality: (0,1)  


**Category**  


Cardinality: (0,n)  


**Related Documents**  
Multiple URLs should be separated by commas.  

Cardinality: (0,n)  

**Distribution**  

Cardinality: (0,n)  

**Size**  
Sizes should be formatted as (e.g.), 52kb, 140mb, 2gb.  


Cardinality: (0,n)  

**Homepage URL**  

Cardinality: (0,1)  

**RSS Feed**  

Cardinality: (0,n)  



### Use Cases  
  
A) Starting from a spreadsheet

Some agencies may initially build or maintain data catalogs through large spreadsheets.  In order to then generate a data.json file from this, simply import the spreadsheet (in the form of a CSV file) into the [Catalog Generator](http://project-open-data.github.com/catalog-generator/), translate the metadata as needed, and then generate an appropriately formatted JSON file.

B) Translating a data file from another schema

If your agency has a JSON catalog with a different metadata schema and need to convert it to the prescribed schema needed for the data.json file, one can import the file into [Catalog Generator](http://project-open-data.github.com/catalog-generator/), adjust the metadata as needed and export the results again as the appropriately formatted JSON file.

C) Utilizing CKAN 

[CKAN](http://www.CKAN.org) is a popular, open-source data catalog.  Even if an agency hasn't begun a data catalog, adopting CKAN can provide a robust and feature-rich solution with which to begin maintaining an internal or external catalog.  In addition to providing an effective means of organizing the agency's data catalog, CKAN provides several opportunities for generating the needed data.json file.  CKAN provides a convenient CSV export that can then be imported into the [Catalog Generator](http://project-open-data.github.com/catalog-generator/) for conversion into an appropriately formatted JSON file.  Alternatively, CKAN provides a JSON API of the data catalog which can then be altered to provide an automatic update for the appropriately formatted JSON file.  

D) Manual translating a data file from another system

Agencies may also manage their data catalogs through various database solutions such as Access, an asset management sytem, document management system, geoportal, or assorted proprietary systems.  Regardless of which system an agency employs, it should include a fundamental export option which allows the catalog to be exported as a CSV file, which can then be imported into the [Catalog Generator](http://project-open-data.github.com/catalog-generator/) for conversation to an appropriately formatted JSON file.  Depending on the solutions' varied further functionality, some of them may also provide APIs which can then be configured to maintain the data.json file.  If not, they may instead support XML and JSON exports, which can then be converted to the proper format.

E) Convert from CSV or JSON to XML or RDFa lite.  

In order to generate appropriately formatted XML or RDFa Lite files, simply import an appropriately formatted CSV or JSON file into the [Catalog Generator](http://project-open-data.github.com/catalog-generator/), ensure that the metadata fields line up, and re-export the file.