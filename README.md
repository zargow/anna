# Project: Anna

## Basic Overview

Anna is a web application for data processing and analysis with an emphasis on automation and control delegation. Users define methods of data retrieval, processing, audits and feedback.

## Goals

#### Network Archetecture
* Utilize Chef Habitat and Docker for deployment/versioning.
* Add Authentication for session approval and application / resource / pool approval.
* Add a system-level data science service (independent from Anna's).
* Use a configuration file to define privleges for users of our system (as opposed to application-specific).
* Use a configuration file to determine routes, server administration settings, deployments styles. 
* Multiple server node support to allow communication on Anna between multiple servers.
* Automated deployment system, that tests builds, reverts to working formats, maintains microservices as seperate builds, and keeps versioning microservices simple with docker containers. 

#### The App (Anna)
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
* Provide methods of extracting data, builds, reports, and importing these as well, for uncommitted users.

## Workflow

#### Early Stages (architecture phase)
* designing tools for data retrieval templates or batch templates.
* defining reporting features.
* microservice definitions, event handling, authentication.
* chef habitat, docker, and app communication services.
* versioning, deployments, all code uses a model-first approach.
* database communication via APIs.
* interactive and centralized settings and control panels.
* data science tools, handling, pushing, etc.
* adding test-level utilities.

#### Mid Stages (design phase)
* adding service-level utilities

#### Final Stages (product complete phase)
* adding more file types and APIs for data retrieval (not JSON, .db, .csv, or .txt).
* adding more reports, graphs, feedback communication tools.
* adding templating tools for data conversion, batches, views, and reports.
* adding internal and external algos, predictive models, notebooks, new ds scripts.


## Use Cases

#### Use case example 1: very automated using best tools
1. ```Retrieval```: Data is uploaded.
2. ```Conversion```: Conversion layout uses metadata to determine which conversion template to use.
3. ```Build```: Conversion data is mapped to custom data build template based on file metadata or conversion template selected.
4. ```Analysis```: Algos add calculations and generate reports based on only build and pre-defined methods.
5. ```Feedback```: Reports are sent to client or customer.

#### Use case example 2: very manual using basic tools
1. ```Retrieval```: Data is uploaded.
2. ```Conversion```: User selects data from file, on pattern or character count style.
3. ```Build```: A manager approves the build, another user creates the build without a template.
4. ```Analysis```: Analyst builds view filtering out outliers
5. ```Feedback```:  scientist writes feedback graph using data, and emails it to the client.

#### Use case example 3: partial use
1. ```Retrieval```: N/A
2. ```Conversion```: N/A
3. ```Build```: Connect to a database, use this database as a build
4. ```Analysis```: run a report of the data
5. ```Feedback```: N/A

#### Summary

There are many more paths with other use cases, but the important use cases are: partial uses, automated uses, and manual uses. Our target users are members of organizations, who need tools to understand their role and place in Anna for their organization. It should also be easy for indivual users by drawing more options for I/O in between the design and product complete phases.

## Technologies

## Resources
http://senecajs.org/getting-started/ -senaca, a template for a microservice project in node.js
