---
layout: default
title: Slash Data Catalog Requirements
permalink: /catalog/
filename: catalog.md
published: false
---

/Data Requirements
------------------

The Open Data Policy requires Agencies to list and describe all agency data that *can* be made publicly available (i.e. there are no valid restrictions to release) in a publicly available open data catalog with common core metadata.  It further requires the catalog to be human-readable and machine-readable.  This guidance describes to agencies steps for implementing this portion of the policy. 

Why this effort
---------------

The data agencies collect and curate is a national treasure. Data from the national weather service and the global positioning system have each given rise to countless products and entire industries, yet much more government data exists, waiting to be tapped of its potential. 

To this end, the digital strategy action item 2.2 [requires](http://www.whitehouse.gov/sites/default/files/omb/egov/digital-government/digital-government.html#existing-data) agencies to catalog and tag their data to make it more easily discoverable to private-sector developers and entrepreneurs.

Through this effort, agencies will begin to tag their data, using common standards, in hopes of building a comprehensive [folksononmy](http://en.wikipedia.org/wiki/Folksonomy) to make government data more easily discoverable. 

Each agency will describe their existing datasets as they see fit using the below described standard, and will make such metadata available at a consistent URL across agencies. Similar to existing practices already in use on the web, such as `sitemap.xml` or `robots.txt`, this will allow developers, both within the government and the public to programmatically discover government data in a machine-readable way.

Machine-Readable Format
-----------------------

All information deemed 'machine-readable' required in this policy must be available in the following formats: JSON, RDFa-Lite and XML.  See this [specification](http://project-open-data.github.com/data-catalog/) for the required schema.  Agencies must post their files at /data.json, /data.html and/or data.xml.  Additionally, the web page which reads and formats these files must be posted at /data/index.html (or data.html).  The files should be updated a minimum of monthly.  It is our intent that future publications of data.gov will simply crawl for agency.gov/data/data.json, data.html (or data.xml) to populate data.gov.

Implementing
------------

To fulfill the requirements of this memorandum, agencies should begin to [describe datasets using the schema.org vocabulary](http://blog.schema.org/). This catalog is to be published in two places. First, as a standalone JSON file at `agency.gov/data.json` and second with RDFa Lite, either embedded within a HTML page which include human readable markups (e.g., `agency.gov/data.html`) or as an XML file (e.g., `agency.gov/data.xml`). 

### JSON

JSON is a lightweight and simple way to represent machine-readable data. It is quickly becoming the *de facto* standard for shuttling data across the internet, fueled primarily by the rise of mobile and APIs. Most if not all modern programing languages can interpret and produce JSON out of the box. 

The JSON representation of the catalog should track directly to the RDFa version, with the exception that JSON keys should not contain the domain prefix (e.g., `dct:title` becomes `title` and `dct:description` becomes simply `description`). Catalogs should be composed of an array of JSON objects, and all fields other than keywords should be a string (where keywords is an array of strings).### RDFa Lite

[RDFa Lite](http://www.w3.org/TR/rdfa-lite/) is a subset of RDFa (Resource Description Framework in Attribute) that provides a common syntax for expressing metadata on websites in a way that computers can understand and begin to formulate knowledge about those data about your organization. RDFa Lite embeds itself in existing, standard HTML pages. For example, if previously a dataset was described as `<h2>Name of Dataset</h2>`, RDFa would extend that markup as  `<h2 property="dct:title">Name of Dataset</h2>` (notice the additional of the property field). This additional metadata is not visible when the page is rendered, and does not affect the page layout or content. It simply provides an additional level of description for search engines, crawlers, and other programatic consumers of your site's content.  It is acceptable for the RDFa-Lite file to contain only the machine readable metadata, but agencies may wish to add human readable content to display the metadata to the public if they so desire.


Generating Machine-Readable Reporting Files
-------------------------------------------

Agencies must follow the provided [specification](http://project-open-data.github.com/data-catalog/).  We have built a [catalog generator](https://github.com/project-open-data/catalog-generator) to assit you in building your catalog and generating .xml, .json, or RDFa Lite files.  

Presentation
------------

Agencies must have present a table/list of each dataset in the /data page.  The /data pages will serve as the authoritative source of agency publicly available data. The page there must be populated with the a list of data sets.  The presentation of this page must contain a table/list of the data in the agencies catalog with at least the following attributes;

* Dataset name
* Dataset description
* URL to the dataset (endpoint)

The page must be populated from the machine readable catalog file (e.g. data.xml or data.json) following the [specification](http://project-open-data.github.com/data-catalog/) described above.  Agencies are encouraged to add functionality to assit end user discoverability.  Additional functions might be sorting, filtering or paging to help make a more digestible list.  Agencies are also encouraged to add more to the standard schema which might further assist end user discoverability and usability (e.g. thumbnails).

Supplemental Information
------------------------

Agencies are encouraged to supplement this requirement  with other information, outreach and tools (e.g. blog posts, github tools, customer engagement tools etc).  Components, bureaus and programs are als encouraged to highlight their work implementing the Policy through their own channels.