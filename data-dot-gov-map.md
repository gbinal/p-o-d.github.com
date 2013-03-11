---
layout: default
title: Schema Mapped to Equivalents
permalink: /data-dot-gov-map/
filename: data-dot-gov-map.md
published: true
---

====================

"Common Core" Required Fields Equivalents
-----------------------------

{.table .table-striped}
Field               | *Data.gov*   | *CKAN* | *RDFa Lite 1.1*  
-------             | -------                 | -------           | ------- 
Title               | *Title*                 | *title*           | [dcterms:title](http://www.w3.org/TR/vocab-dcat/#property--title-1)    
Description         | *Description*           | *notes*                | [dcterms:description](http://www.w3.org/TR/vocab-dcat/#property--description-1) 
Download URL        | *Access Point*          | *resources\[url\]*                | [dcat:accessURL](http://www.w3.org/TR/vocab-dcat/#property--access-download)
Format              | *Media Format*          | *resources\[format\]*                | [dcterms:format](http://www.w3.org/TR/vocab-dcat/#property--format)      
Tags                | *Keywords*              | *tags*                | [dcat:keyword](http://www.w3.org/TR/vocab-dcat/#property--keyword-tag)    
Last Update         | *Date updated*          | *revision_timestamp*                | [dcterms:modified](http://www.w3.org/TR/vocab-dcat/#property--update-modification-date-1)
Publisher           | *Agency Name*           | *owner_org*                | [foaf:Organization](http://www.w3.org/TR/vocab-dcat/#class--organization-person)
Contact Name        | *Contact Name*          | *maintainer*                | [foaf:Person](http://www.w3.org/TR/vocab-dcat/#class--organization-person)
Contact Email       | *Contact Email Address* | *maintainer_email*                | [foaf:mbox](http://xmlns.com/foaf/spec/#term_mbox)
Unique Identifier   | *User Generated ID*     | *id*                | [dcterms:identifier](http://www.w3.org/TR/vocab-dcat/#property--identifier)
Public Access Level | *n/a*                   | *n/a*             | *n/a*

"Common Core" Required if Applicable Fields
-------------------------------------------

{.table .table-striped}
Field               | *Data.gov*   | *CKAN* | *RDFa Lite 1.1*
-------             | -------                 | -------           | ------- 
Documentation URL   | *Data Dictionary*       | *n/a*                | [dcat:dataDictionary](http://www.w3.org/TR/vocab-dcat/#property--data-dictionary)
Endpoint            | *Access Point*          | *n/a*                | [dcat:webService](http://www.w3.org/TR/vocab-dcat/#class--webservice) \* 
License             | *Dataset license agreement URL* | *license_id*        | [dcterms:license](http://www.w3.org/TR/vocab-dcat/#property--license-1)
Spatial             | *Geographic scope*      | *n/a*                | [dcterms:spatial](http://www.w3.org/TR/vocab-dcat/#property--spatial-geographical-coverage)
Temporal      	    | *Period of Coverage*    | *n/a*                | [dcterms:temporal](http://www.w3.org/TR/vocab-dcat/#property--temporal-coverage)

Expanded Fields
---------------

{.table .table-striped}
Field               | *Data.gov*   | *CKAN* | *RDFa Lite 1.1*
-------             | -------                 | -------           | ------- 
Release Date        | *Date Released*         | *n/a*                | [dcterms:issued](http://www.w3.org/TR/vocab-dcat/#property--release-date)
Frequency           | *Frequency*             | *n/a*                | [dcterms:accrualPeriodicity](http://www.w3.org/TR/vocab-dcat/#property--frequency)   
Language            | *n/a*                   | *n/a*                | [dcat:language](http://www.w3.org/TR/vocab-dcat/#property--language-1)     
Granularity         | *Geographic Granularity* | *n/a*                | [dcat:granularity](http://www.w3.org/TR/vocab-dcat/#property--granularity)
Data Quality        | *Data Quality*          | *n/a*                | [xsd:boolean](http://www.w3.org/TR/xmlschema-2/#boolean)
Category            | *Subject Area*          | *groups*                | [dcat:theme](http://www.w3.org/TR/vocab-dcat/#property--theme-category)  
Related Documents   | *Reference for Technical Documentation* | *n/a*                | [dcterms:references](http://www.w3.org/TR/vocab-dcat/#property--related-documents)
Distribution        | *Dataset Group Name*    | *n/a*                | [dcat:distribution](http://www.w3.org/TR/vocab-dcat/#property--dataset-distribution)
Size                | *File Size*             | *n/a*                | [dcat:size](http://www.w3.org/TR/vocab-dcat/#property--size)
Homepage URL        | *n/a*	                  | *url*                | [foaf:homepage](http://www.w3.org/TR/vocab-dcat/#property--homepage)
RSS Feed            | *Access Point*          | *n/a*                | [dcat:feed](http://www.w3.org/TR/vocab-dcat/#Class:_Feed) \* 

\*When combined with _accessURL_, _format_, and _size_.
