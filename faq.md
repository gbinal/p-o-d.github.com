---
layout: default
title: Frequently Asked Questions
permalink: /faq/
filename: faq.md
published: false
---

### Acquisition

* What resources are available to help agencies incorporate the policy requirements into their acquisition processes?  
  * Sample acquisition language may be found at {LINK}

### Information Systems

* Who is in charge of Project Open Data?  
  * The White House owns Project Open Data, and will directly manage a select set of repos while a program management office (PMO) in the General Services Administration (GSA) will delegate management of other individual repos on behalf of the White House, as well as provide daily oversight and user support for the Project.

* Who can participate in Project Open Data?  
  * Anyone – Federal employees, contractors, developers, the general public – can view and contribute to Project Open Data. (Set up a GitHub user account to get started).

* Can I create a new page (i.e., repo) within Project Open Data?
 * Creation of a new repo within Project Open Data is controlled by the project PMO. If you would like to create a new repo, please (insert instructions).

* How can I see whether my suggested change (i.e., pull request) was accepted?
 * (insert answer)

* How long will I have to wait to get a response to my suggested change (i.e., pull request)?
 * Release cycles vary from repo to repo. Check out the readme file of the repo where you submitted a pull request to see how often code pushes and updates are done. 

### Information Systems

* How can agencies meet the requirement that new systems must "facilitate extraction of data in multiple formats and for a range of uses as internal and external needs change, including potential uses not accounted for in the original design"?
 * CHECK TO SEE IF THE POLICY LANGUAGE CHANGED
 
### IRM Strategic Plans
 
* When will additional guidance on IRM strategic plans be released?
 * CHECK TO SEE IF THE POLICY LANGUAGE CHANGED
 
### Machine Readable and Open Formats

* Does PDF meet the “machine readable and open format” requirement?
 * While ISO 32000 is an open standard, the Portable Document Format (PDF) does not achieve the same level of openess as CSV, XML, JSON and other generic formats.

### Metadata

* What is the relationship of the metadata standard (specifically) to NIEM, ISE, FGDC, and other existing (especially official) government data standards?
 * The core metadata schema at {LINK} is based on existing vocabularies and easily mapped to NIEM, Information Sharing Enviroment, and FGDC.

* What is a "persistent identifier"?
 * A persistent identifier is a unique label assigned to digital objects or data files that is managed and kept up to date over a defined time period (e.g., Unique Investment Identifiers).

* Who established the core metadata schema?
 * The core metadata schema was the result of recommendations from a governmenwide Metadata Working Group at Data.gov combined with research of existing public schemas for data catalogs.  Most of the elements trace their roots to the Dublin Core Library.
 
* How can I recommend changes and improvements to the metadata schema?

* Can I extend the metadata schema beyond the terms specified at {LINK} ?
 * Yes, if your data management process includes rich metadata specific to the mission of your agency or the Line of Business your agency participates, pubishing additional metadata that makes your data more usefull to the public is welcomed and encouraged.  Note that Data.gov will be harvesting only the metadata in this published schema unless specific arrangements are in place (e.g. geospatial FGDC/ISO).
 

### Security, Privacy and Data Quality

* Who is reponsible for insuring that datasets published in the agency.gov/data page (and subsequently Data.gov) meet each agencies requirements for security and privacy and quality?
 * Each agency is responsible for ALL data made public.
 
* How can I contact the Data.gov staff for assistance in conducting mosaic effect reviews?
 * For general questions about Data.gov, please contact http://www.data.gov/contact-us . For specific information about the mosaic effect, please contact the Data.gov PMO at GSA.


### Public Data Listing

* What is the value to the government to place metadata at agency.gov/data?
 * Having the metadata available at the agency level provides agencies with a self-managed publishing capability.  In addition, having the metadata in a machine-readable format opens the possibility that major search engines will index these metadata in a manner similar to site maps and allow the public to discover public data across the government using a search tool of their choice.

* How will agency.gov/open, /developer, and /data pages work together?
 * The agency.gov/open page contains informational regards an agencies contributions to Open Government, while the /developer and /data pertains to APIs and Open Data. All three pages contribute to an open and transparent government in the United States.

* What is the relationship of the /data page and public data listing to Data.gov and how will this impact current Data.gov processes?
 * In the near term, Data.gov will continue it's current dataset publishing process.  As agencies deploy agency.gov/data page, the publishing process will become a harvesting of metadata from the agencies web site.

* Are redirects allowed for /data pages?
 * Yes, redirects are useful for agencies who need alternatives for their Content Management Systems (CMSs).
 
* What options exist for hosting the /data.json file specifically at agency.gov/data.json?  
1. For websites that are composed of static html, simiply host the data.json file at the designated location.  
2. ...
3. ...
4. ...
5. ...
 
* How do I get started building this /data file?
 * Datagov will (when possible) help agencies get started by creating a /data file for each agency containing the metadata in the correct syntax.  The agency will then begin to manage that file for future publishing of datasets.
  
* How should I manage this /data file?
 * A wide variety of tools are available to manage a data catalog, be it public facing or for internal data managements.  Managing the records of metadata in the file can be managed by databases, spreadsheets, or even text editors.  Data management systems should be able to export the metadata either in the desired format or simply mapped with tools.
 
* What formats are required/recommended for the agency.gov/data file?
 * There are several syntaxes that may be used when publishing the data file.  The syntax that is required to make the data readily available to developers is JSON (JavaScript Object Notation).  It is recommended that agencies also create a data.html file and use RDFa-Lite (Resource Description Framework) to mark-up the metadata using the schema located at {link}.  The RDFa-Lite file will be easily consumed by major search engines and applications and make you data easier to find by the public.  A third alternative for populating your metadata file is XML (eXtensible Markup Language).  Agencies are encouraged to maintain all three version of the metadata file.  Tools are available to transform any instance of the file into the alternative formats.
 
 

### Agency participation with Open Data

* What are some of the ways that agencies can become more involved with Open Data
 * Having a contact point at the agency who can answer questions and received comments about published data is extremely important to making your data more open and valuable to the public.  This contact point can be centralized at the agency level, but having someone close to the source of the data who understands it well enough to help the public take full advantage of available data is extremely valuable.

### Scope 

* How should agencies prioritize making improvements to existing systems and data?
...Agencies should also ensure continuity of access to the data by involving primary users in the changes.

* Which agencies are required to implement this policy?

### Timeline
How long do agencies have to implement the policy?