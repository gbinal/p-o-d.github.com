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
Field               |JSON            | RDFa Lite  | | *Data.gov Equivalent*  
-------             | -------------------  | --------------  | | ------- 
Title               | title           | [dct:title](http://dublincore.org/documents/2012/06/14/dcmi-terms/?v=terms#terms-title)  | | *Title*                
Description         | description     | [dct:description](http://dublincore.org/documents/2012/06/14/dcmi-terms/?v=terms#terms-description)  | | *Description*          
Documentation URL   | dataDictionary  | [dcat:dataDictionary](http://www.w3.org/TR/vocab-dcat/#property--data-dictionary)  | | *Data Dictionary*      
URL                 | accessURL       | [dcat:accessURL](http://www.w3.org/TR/vocab-dcat/#property--access-download)  | | *Access point*         
Format              | format          | [dcterms:format](http://www.w3.org/TR/vocab-dcat/#property--format)  | | *Media Format*         
Tags                | keywords        | [dcat:keyword](http://www.w3.org/TR/vocab-dcat/#property--keyword-tag)  | | *Keywords*             
Last Update         | modified        | [dcterms:modified](http://www.w3.org/TR/vocab-dcat/#property--update-modification-date-1)  | | *Date updated*         
Publisher           | organization    | [foaf:Organization](http://xmlns.com/foaf/spec/#term_Organization)  | | *Agency Name*          
Contact Name        | person           | [foaf:Person](http://xmlns.com/foaf/spec/#term_Person)  | | *Contact Name*         
Contact Email       | mbox  	         | [foaf:mbox](http://xmlns.com/foaf/spec/#term_mbox)  | | *Contact Email Address*
Public              | public          | [xsd:boolean](http://www.w3.org/TR/xmlschema-2/#boolean)  | | *n/a*                  


"Common Core" Required if Applicable Fields
-------------------------------------------

{.table .table-striped}
Field               |JSON            | RDFa Lite  | *Data.gov Equivalent*  
-------             | -------------------  | --------------  | ------- 
License             | license         | [dcterms:license](http://www.w3.org/TR/vocab-dcat/#property--license-1)  | *Dataset license agreement URL* 
Spatial  	    | spatial 	       | [dcterms:spatial](http://www.w3.org/TR/vocab-dcat/#property--spatial-geographical-coverage)  | *Geographic scope*     
Temporal	    | temporal	       | [dcterms:temporal](http://www.w3.org/TR/vocab-dcat/#property--temporal-coverage)  | *Period of Coverage*   

Expanded Fields
---------------

{.table .table-striped}
Field               | JSON                  | RDFa Lite  | *Data.gov Equivalent*   
------              | -------------------   | ----                  | --------
Release Date        | issued                | [dct:issued](http://dublincore.org/documents/2012/06/14/dcmi-terms/?v=terms#issued)  | *Date Released*         
Frequency           | accrualPeriodicity    | [dct:accrualPeriodicity](http://purl.org/dc/terms/accrualPeriodicity)  | *Frequency*             
Unique Identifier   | identifier            | [dcterms:identifier](http://www.w3.org/TR/vocab-dcat/#property--identifier)  | *User Generated ID*     
Language            | language              | [dcat:language](http://www.w3.org/TR/vocab-dcat/#property--language-1)  | *n/a*                   
Granularity         | granularity           | [dcat:granularity](http://www.w3.org/TR/vocab-dcat/#property--granularity)  | *Geographic Granularity*  
Data Quality        | dataQuality           | [dcat:dataQuality](http://www.w3.org/TR/vocab-dcat/#property--data-quality)  | *Data Quality*          
Category            | theme                 | [dcat:theme](http://www.w3.org/TR/vocab-dcat/#property--theme-category)  | *Subject Area*          
Related Documents   | references            | [dcterms:references](http://purl.org/dc/terms/references)  | *Reference for Technical Documentation* 
Distribution        | distribution          | [dcat:distribution](http://www.w3.org/ns/dcat#distribution)  | *Dataset Group Name*    
Size                | size                  | [dcat:size](http://www.w3.org/TR/vocab-dcat/#property--size)  | *File Size*             
Download URL        | download              | [dcat:download](http://www.w3.org/TR/vocab-dcat/#class--download)  | *Access Point*          
Homepage URL        | homepage	            | [foaf:homepage](http://xmlns.com/foaf/spec/#term_homepage)  | *n/a*	
Endpoint            | WebService            | [dcat:webService](http://www.w3.org/TR/vocab-dcat/#class--webservice)  | *Access Point*          
RSS Feed            | Feed                  | [dcat:feed](http://www.w3.org/TR/vocab-dcat/#Class:_Feed)  | *Access Point*          


