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
Field               | *Data.gov*   | *CKAN* | *RDFa Lite 1.1*  | *Schema.org*
-------             | -------                 | -------           | ------- | ------- 
Title               | *Title*                 | *title*           | [dcterms:title](http://www.w3.org/TR/vocab-dcat/#property--title-1)    | *sdo:name*
Description         | *Description*           | *notes*                | [dcterms:description](http://www.w3.org/TR/vocab-dcat/#property--description-1) | *sdo:description*
Download URL        | *Access Point*          | *resources\[url\]*                | [dcat:accessURL](http://www.w3.org/TR/vocab-dcat/#property--access-download) | *sdo:contentUrl*
Format              | *Media Format*          | *resources\[format\]*                | [dcterms:format](http://www.w3.org/TR/vocab-dcat/#property--format)      | *sdo:encodingFormat*
Tags                | *Keywords*              | *tags*                | [dcat:keyword](http://www.w3.org/TR/vocab-dcat/#property--keyword-tag)    | *sdo:keywords*
Last Update         | *Date updated*          | *revision_timestamp*                | [dcterms:modified](http://www.w3.org/TR/vocab-dcat/#property--update-modification-date-1) | *sdo:dateModified* 
Publisher           | *Agency Name*           | *owner_org*                | [dcat:publisher](http://www.w3.org/TR/vocab-dcat/#property--publisher-1) | *sdo:publisher*
Contact Name        | *Contact Name*          | *maintainer*                | [foaf:Person](http://www.w3.org/TR/vocab-dcat/#class--organization-person) | *sdo:Person*
Contact Email       | *Contact Email Address* | *maintainer_email*                | [foaf:mbox](http://xmlns.com/foaf/spec/#term_mbox) | *n/a*
Unique Identifier   | *User Generated ID*     | *id*                | [dcterms:identifier](http://www.w3.org/TR/vocab-dcat/#property--identifier) | *n/a*
Public Access Level | *n/a*                   | *n/a*             | *n/a* | *n/a*

"Common Core" Required if Applicable Fields
-------------------------------------------

{.table .table-striped}
Field               | *Data.gov*   | *CKAN* | *RDFa Lite 1.1* | *Schema.org*
-------             | -------                 | -------           | -------  | ------- 
Documentation URL   | *Data Dictionary*       | *n/a*                | [dcat:dataDictionary](http://www.w3.org/TR/vocab-dcat/#property--data-dictionary) | *n/a*
Endpoint            | *Access Point*          | *n/a*                | [dcat:webService](http://www.w3.org/TR/vocab-dcat/#class--webservice) \*  | *n/a*
License             | *Dataset license agreement URL* | *license_id*        | [dcterms:license](http://www.w3.org/TR/vocab-dcat/#property--license-1) | *n/a*
Spatial             | *Geographic scope*      | *n/a*                | [dcterms:spatial](http://www.w3.org/TR/vocab-dcat/#property--spatial-geographical-coverage) | *ds:spatialCoverage*
Temporal      	    | *Period of Coverage*    | *n/a*                | [dcterms:temporal](http://www.w3.org/TR/vocab-dcat/#property--temporal-coverage) | *ds:temporalCoverage*

Expanded Fields
---------------

{.table .table-striped}
Field               | *Data.gov*   | *CKAN* | *RDFa Lite 1.1* | *Schema.org*
-------             | -------                 | -------           | -------  | ------- 
Release Date        | *Date Released*         | *n/a*                | [dcterms:issued](http://www.w3.org/TR/vocab-dcat/#property--release-date) | *sdo:datePublished*
Frequency           | *Frequency*             | *n/a*                | [dcterms:accrualPeriodicity](http://www.w3.org/TR/vocab-dcat/#property--frequency)    | *n/a*
Language            | *n/a*                   | *n/a*                | [dcat:language](http://www.w3.org/TR/vocab-dcat/#property--language-1)     | *sdo:inLanguage*
Granularity         | *Geographic Granularity* | *n/a*                | [dcat:granularity](http://www.w3.org/TR/vocab-dcat/#property--granularity) | *n/a*
Data Quality        | *Data Quality*          | *n/a*                | [xsd:boolean](http://www.w3.org/TR/xmlschema-2/#boolean)  | *n/a*
Category            | *Subject Area*          | *groups*                | [dcat:theme](http://www.w3.org/TR/vocab-dcat/#property--theme-category)   | *sdo:about*
Related Documents   | *Reference for Technical Documentation* | *n/a*                | [dcterms:references](http://www.w3.org/TR/vocab-dcat/#property--related-documents) | *n/a*
Distribution        | *Dataset Group Name*    | *n/a*                | [dcat:distribution](http://www.w3.org/TR/vocab-dcat/#property--dataset-distribution) | *ds:distribution*
Size                | *File Size*             | *n/a*                | [dcat:size](http://www.w3.org/TR/vocab-dcat/#property--size) | *sdo:contentSize*
Homepage URL        | *n/a*	                  | *url*                | [foaf:homepage](http://www.w3.org/TR/vocab-dcat/#property--homepage) \*\*  | *sdo:url*
RSS Feed            | *Access Point*          | *n/a*                | [dcat:feed](http://www.w3.org/TR/vocab-dcat/#Class:_Feed) \*  | *n/a*

\*When combined with _accessURL_, _format_, and _size_.

\*\*In DCAT, *foaf:homepage* refers to the catalog homepage, while in the "common core" metadata it refers to the dataset homepage.
