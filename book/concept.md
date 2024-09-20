# The KnowLedger Concept

The KnowLedger project is about the creation of an ecosystem to support the varied and ever evolving needs of the 
research community.  As such, the project is focused on what needs to be built as part of the ecosystem, and how should
it be run so that the research community is part of the development team and can enable what they wish for a notebook 
that fits their research needs.

KnowLedger, then is designed around the needs of research, that being:
- a place to capture research data digitally at birth (including a log of research activities)
- an interface that allows easy annotation (text, audio, video)
- a platform that provides data analysis and workflow tools (through integrated modules)
- a system that integrates with online research resources ('visual' APIs)
- a resource that stores data semantically (for knowledge mining)
- a notebook that allows sharing of workflows, protocols, metadata standards 
- an ecosystem that is focused on data management, trust, and enabling collaboration

Our approach to the KnowLedger concept is to:
- Develop the KnowLedger software (in Python) to be open platform upon which data can be collected, managed, processed, 
  annotated, analyzed, published, and archived
- Use of a generic but flexible data container – the SciData framework in JSON-LD – to store research data, create 
  sharable templates (experiments, resources, raw and processed data), adapters (to connect online resources),
  and converters (to import data from online systems)
- Modularize the ecosystem around this approach to encourage tool development, resource access, workflow monitoring/control 
  by developing a JSON-LD framework for the data infrastructure
- Develop an open framework for persistent identifier (PID) assignment to data and resources in alignment with the 
  recently published strategy for PID development and current PID systems
- Provide open access to community-built data templates, resource modules, and workflow templates via a network of 
  GitHub repositories that can be centrally linked though persistent identifiers
- Provide documentation of all parts of the ecosystem and delineate common best practices for development of code 
  in support of resources
- Engage with the International Unions, CODATA/ISC and scientific societies to promote and guide communities
- Promote the FAIR principles, CARE, digital Data Management Plans (DMPs) and open science

The project goals, which are intended to focus the development of KnowLedger, are to:
- Remove barriers to the collection of rich metadata along with experimental data, analysis and results 
  (e.g. help researchers get better metadata from instruments, sensors, surveys, etc.)
- Promote community development of minimal metadata standards for recording instrument, experiment, sample, 
  workflow, analysis metadata, etc.
- Enable community development/adoption of best practices for workflows, analysis and data reporting
- Encourage data sharing, data reuse, and collaboration to identify interoperability challenges and develop 
  approaches to tracking data provenance and versioning of datasets
- Define/integrate metrics for data quality, data reliability, data provenance, and data integrity
- Generally, adopt best practices, community standards, and open specifications where available and appropriate

Technically, we are focused on using GitHub and Docker containers to create an ecosystem of resources that can be 
integrated via a Python application, KnowLedger.  Through a set of project GitHub repositories, and set of community
repositories we will build the ecosystem with community input using the functionality of GitHub, such as issues, projects,
wiki and actions.  The KnowLedger application will be deployed initially as docker images so that researchers can play
with it locally, providing feedback in the beta phase of this project.  Further deployment options for KnowLedger will
be based on community feedback.

Additionally, the data saved in KnowLedger as well as templates for data, workflows, analysis and other parts of the system
will be captured in JSON-LD ([JSON for Linked Data](https://www.w3.org/TR/json-ld/)).  This is an encoding of the 
Resource Description Framework (RDF), used to represent data semantically.  The SciData framework will be used to 
format the data in JSON-LD and SciData will be evaluated for other parts of the system to evaluate if it can be extended
for all needs, or if other frameworks are needed.  As the data format is JSON-LD, [MongoDB](https://www.mongodb.com/) 
will be used as the database for storing KnowLedger data, and provided as part of the Docker container for KnowLedger, 
minimizing technical requirements to deploy KnowLedger.

For more information, a visual representation of the project ecosystem can be found [here](ecosystem.md).  You can also
download a copy of the project proposal [here](files/knowledger_proposal.pdf)

**Stuart Chalk, KnowLedger Project PI** &bullet; [schalk@unf.edu](mailto:schalk@unf.edu) &bullet; [ORCID](https://orcid.org/0000-0002-0703-7776)