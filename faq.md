---
layout: default
title: Frequently Asked Questions
permalink: /faq/
filename: faq.md
published: false
---

## Project Open Data

### What problem does this solve?

Technology moves much faster than policy ever could.  Often when writing policy for technology, agencies are stuck w/ outdated methods as soon as they publish new policies.

### How does it solve that problem?

This Project is meant to be a living document so that collaboration in the open data ecosystem is fostered and the continual update of technology pieces that affect update can happen on a more rapid pace.

### Where do I come in?

Help the United States Government make its Open Data policy better by collaborating.  Please suggest enhancements by editing the content here, or add tools that help anyone open data (See 'How can I contribute'). 

### How can I contribute?

This project constitutes a collaborative work ("open source"). Federal employees and members of the public are encouraged to improve the project by contributing. This can be done in two ways:

#### Easy

1. Click the "Improve this content" button in the top right corner of any page.
2. Make changes as you would normally.
3. Click "Submit".
4. You change should appear once approved.

*Note: You may need to [create a free GitHub account](https://github.com/signup/free) if you do not already have one.*

#### Advanced

1. Configure git by using this [basic tutorial](https://help.github.com/articles/set-up-git) or by downloading the [GitHub for Mac](http://mac.github.com/)/[GitHub for Windows](http://windows.github.com/) and optionally [Mou](http://mouapp.com/).
2. [Fork](https://help.github.com/articles/fork-a-repo) the project.
3. Make changes as you would normally using the tools installed in step #1.
4. Push the changes back to your fork.
5. Submitting a pull request to this repository.
6. You change should appear once approved.

*Note: All contributors retain the original copyright to their contribution, but by contributing to this project, you grant a world-wide, royalty-free, perpetual, irrevocable, non-exclusive, transferable license to all users under the terms of the license(s) under which this project is distributed.*

### Can I use the project's content or source code elsewhere?

The project [as originally published](#) constitutes a work of the United States Government and is not subject to domestic copyright protection under 17 USC § 105. Subsequent contributions by members of the public, however, retain their original copyright.

In order to better facilitate collaboration, the content of this project is licensed under the [creative commons 3.0 license](http://creativecommons.org/licenses/by/3.0/us/deed.en_US), and the underlying source code used to format and display that content is licensed under the [MIT license](http://opensource.org/licenses/mit-license.php). 

### Who can participate in Project Open Data?  

Anyone – Federal employees, contractors, developers, the general public – can view and contribute to Project Open Data.

### Are my interactions to this project subject to any special privacy considerations?

Comments, pull requests and any other messages received through this repository may be subject to the [Presidential Records Act](http://www.archives.gov/about/laws/presidential-records.html) and may be archived. Learn more at http://WhiteHouse.gov/privacy

### Who is in charge of Project Open Data?  

Ultimately? You. While the White House founded and continues to oversee the project, Project Open Data is a collaborative work — commonly known as "open source" — and is supported by the efforts of an entire community. See the "how to contribute" section above to learn more.

At the onset, the General Services Administration is here to provide daily oversight and support, but over time, it is our vision that contributors both inside and outside of government can be empowered to take on additional leadership roles.

### Can I create a new page?

Yes! Simply follow the "advanced" instructions above to submit a pull request.

### How can I see whether my suggested change (i.e., pull request) was accepted?

(insert answer)

### How long will I have to wait to get a response to my suggested change (i.e., pull request)?

Release cycles vary from repo to repo. Check out the readme file of the repo where you submitted a pull request to see how often code pushes and updates are done. 

## Acquisition

### What resources are available to help agencies incorporate the policy requirements into their acquisition processes?  

Sample acquisition language may be found at {LINK}

## Information Systems

### How can agencies meet the requirement that new systems must "facilitate extraction of data in multiple formats and for a range of uses as internal and external needs change, including potential uses not accounted for in the original design"?

CHECK TO SEE IF THE POLICY LANGUAGE CHANGED
 
## IRM Strategic Plans
 
### When will additional guidance on IRM strategic plans be released?

Guidance on IRM strategic plans will be released in early 2013.

## Machine Readable and Open Formats

### Does PDF meet the “machine readable and open format” requirement?

While ISO 32000 is an open standard, the Portable Document Format (PDF) does not achieve the same level of openness as CSV, XML, JSON and other generic formats.

## Metadata

### What is the relationship of the metadata standard (specifically) to NIEM, ISE, FGDC, and other existing (especially official) government data standards?

The [core metadata schema](http://gsa-ocsit.github.com/project-open-data.github.com/schema/) is based on existing vocabularies and easily mapped to NIEM, Information Sharing Environment, and FGDC.

### What is a "persistent identifier"?

A persistent identifier is a unique label assigned to digital objects or data files that is managed and kept up to date over a defined time period (e.g., Unique Investment Identifiers).

### Who established the core metadata schema?

The core metadata schema was the result of recommendations from a government-wide Metadata Working Group at Data.gov combined with research of existing public schemas for data catalogs.  Most of the elements trace their roots to the Dublin Core Library.
 
### How can I recommend changes and improvements to the metadata schema?

Submit a pull request for the core metadata schema. 

### Can I extend the metadata schema beyond the terms specified in the [core metadata schema](http://gsa-ocsit.github.com/project-open-data.github.com/schema/)?

Yes, if your data management process includes rich metadata specific to the mission of your agency or the Line of Business your agency participates, publishing additional metadata that makes your data more useful to the public is welcomed and encouraged.  Note that Data.gov will be harvesting only the metadata in this published schema unless specific arrangements are in place (e.g. geospatial FGDC/ISO).
 

## Security, Privacy and Data Quality

### Who is responsible for insuring that datasets published in the agency.gov/data page (and subsequently Data.gov) meet each agency's requirements for security and privacy and quality?

Each agency is responsible for ALL data made public.
 
### How can I contact the Data.gov staff for assistance in conducting mosaic effect reviews?

For general questions about Data.gov, please contact http://www.data.gov/contact-us. For specific information about the mosaic effect, please contact the Data.gov PMO at GSA.


## Public Data Listing

### What is the value to the government in placing metadata at agency.gov/data?

Having the metadata available at the agency level provides agencies with a self-managed publishing capability.  In addition, having the metadata in a machine-readable format opens the possibility that major search engines will index these metadata in a manner similar to site maps and allow the public to discover public data across the government using a search tool of their choice.

### How will agency.gov/open, /developer, and /data pages work together?

The agency.gov/open page contains informational regards an agencies contributions to Open Government, while the /developer and /data pertains to APIs and Open Data. All three pages contribute to an open and transparent government in the United States.

### What is the relationship of the /data page and public data listing to Data.gov and how will this impact current Data.gov processes?

In the near term, Data.gov will continue its current dataset publishing process.  As agencies deploy agency.gov/data pages, the publishing process will become a harvesting of metadata from the agencies web site.

### Are redirects allowed for /data pages?

No, the files should be located at agency.gov/data web space.  Each agency should populate files named agency.gov/data.json, agency.gov/data.html and agency.gov/data.xml .
 
### What options exist for hosting the /data.json file specifically at agency.gov/data.json?  

1. For websites that are composed of static html, simply host the data.json file at the designated location.  
2. If needed, one may also host the file by using /data.json/index.html to provide the same functionality.  
3. Sites that utilize Wordpress may modify and employ the opensourced [Datafiles Wordpress Plugin](https://github.com/GSA/datafiles-wordpress-plugin).  
4. Sites that utilize Drupal may modify and employ the opensourced [Digital Strategy Drupal Module](https://github.com/FCC/digital_strategy).  

 
### How do I get started building this /data file?

Data.gov will (when possible) help agencies get started by creating a /data file for each agency containing the metadata in the correct syntax.  The agency will then begin to manage that file for future publishing of datasets.
  
### How should I manage this /data file?

A wide variety of tools are available to manage a data catalog, be it public facing or for internal data managements.  Managing the records of metadata in the file can be managed by databases, spreadsheets, or even text editors.  Data management systems should be able to export the metadata either in the desired format or in one which may be simply mapped with [tools](http://labs.data.gov).
 
### What formats are required/recommended for the agency.gov/data file?

There are several syntaxes that may be used when publishing the data file.  The syntax that is required to make the data readily available to developers is JSON (JavaScript Object Notation).  It is recommended that agencies also create a data.html file and use RDFa-Lite (Resource Description Framework) to mark-up the metadata using the [core metadata schema](http://project-open-data.github.com/schema/).  The RDFa-Lite file can be easily consumed by major search engines and applications and make you data easier to find by the public.  A third alternative for populating your metadata file is XML (eXtensible Markup Language).  Agencies are encouraged to maintain all three version of the metadata file.  [Tools](http://labs.data.gov) are available to transform any instance of the file into the alternative formats.

## Agency participation with Open Data

### What are some of the ways that agencies can become more involved with Open Data?

Having a contact point at the agency who can answer questions and received comments about published data is extremely important to making your data more open and valuable to the public.  This contact point can be centralized at the agency level, but having someone close to the source of the data who understands it well enough to help the public take full advantage of available data is extremely valuable.

## Scope 

### How should agencies prioritize making improvements to existing systems and data?

Agencies should regularly add to and improve the entries in their data catalog, as well as also ensuring continuity of access to the data by involving primary users in the changes.

### Which agencies are required to implement this policy?

All executive agencies.  

## Timeline

### How long do agencies have to implement the policy?

Agencies are required to implement the data policy within six months.