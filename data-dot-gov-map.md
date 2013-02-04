---
layout: default
title: Schema Mapped to Data.gov Equivalent
permalink: /data-dot-gov-map/
filename: data-dot-gov-map.md
published: true
---

====================

"Common Core" Required Fields
-----------------------------

{.table .table-striped}
Field               | *Data.gov Equivalent*  
-------             | ------- 
Title               | *Title*                
Description         | *Description*          
Documentation URL   | *Data Dictionary*      
URL                 | *Access point*         
Format              | *Media Format*         
Tags                | *Keywords*             
Last Update         | *Date updated*         
Publisher           | *Agency Name*          
Contact Name        | *Contact Name*         
Contact Email       | *Contact Email Address*
Public              | *n/a*                  


"Common Core" Required if Applicable Fields
-------------------------------------------

{.table .table-striped}
Field               |JSON            | RDFa Lite  | *Data.gov Equivalent*  
-------             | -------------------  | --------------  | ------- 
License             | license         | [dcterms:license](http://www.w3.org/TR/vocab-dcat/#property--license-1)  | *Dataset license agreement URL* 
Spatial        | spatial 	       | [dcterms:spatial](http://www.w3.org/TR/vocab-dcat/#property--spatial-geographical-coverage)  | *Geographic scope*     
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


