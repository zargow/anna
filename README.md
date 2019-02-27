# Project: Anna

## Basic Overview

Anna is a web application for data processing and analysis with an emphasis on automation and control delegation. Users define methods of data retrieval, processing, audits and feedback.

## Goals

#### Network infrastructure
* Utilize Chef Habitat and Docker for deployment/versioning.
* Add Authentication for session approval and application / resource / pool approval.
* Add a system-level data science service (independent from Anna's).
* Use a configuration file to define privleges for users of our system (as opposed to application-specific).
* Use a configuration file to determine routes, server administration settings, deployments styles. 
* Multiple server node support to allow communication on Anna between multiple servers.
* Automated deployment system, that tests builds, reverts to working formats, maintains microservices as seperate builds, and keeps versioning microservices simple with docker containers. 

#### Anna (app)
* Code a microservice style application using NodeJS, postgreSQL, Vue.js, and js on jupyter notebooks.
* Create a data retrieval process that reads common file types with API alternatives.
* Create a data conversion process that includes a template editor, to add files  
* Provide a data build process that uses build tables and views to create new build views.
* Provide a data reports process that uses web components, grids, notebooks, and PDFs containers.
  ``` Anna does not provide PDF edit support for reports ```
* Provide administration controls to organizations for setting responsbilities and procedures.
* Always consider the integrity, usability, performance, and cost of different kinds of data moves.
* Development workflow should match "workflow: end" below and maitenance should be seperated by microservice.
* Provide a science-based dashboard that can outline time-sensitive tasks, charts, other widgets.

## Workflow

#### Early Stages
* designing tools for data retrieval templates or batch templates.
* defining reporting features.
* microservice definitions, event handling, authentication.
* chef habitat, docker, and app communication services.
* versioning, deployments, all code uses a model-first approach.
* database communication via APIs.
* interactive settings and control panels.
* data science tools, handling, pushing, etc.

#### Final Stages
* adding more file types and APIs for data retrieval (not JSON, .db, .csv, or .txt).
* adding more reports, graphs, feedback communication tools.
* adding templating tools for data conversion, batches, views, and reports.
* adding internal and external algos, predictive models, notebooks, new ds scripts.


## Life Cycle of Data 

#### Use Case 1: very automated
1. Retrieval: Data is uploaded.
2. Conversion: Conversion layout uses metadata to determine which converesion template to use.
3. Build: Conversion data is mapped to custom data build template based on file metadata or conversion template selected.
4. Analysis: Algos add calculations and generate reports based on only build and pre-defined methods.
5. Feedback: Reports are sent to client or customer.

This could be entirely automated from file retrieval to feedback reports, but its more likely certain processes fail and require manual attention, or that roles are segregated and require completion to begin the next task.

#### Use Case 2: very manual


#### Data Retrieval
No formatted files neccessary! As long as your files contain common encoding patterns, Anna will provide useful templating tools to help automate your data retrieval tasks.
