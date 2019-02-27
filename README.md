# Project: Anna

## Basic Overview

Anna is a web application for data processing and analysis with an emphasis on automation and control delegation. Users define methods of data retrieval, processing, audits and feedback.

## Projected Work Load

#### Start-Up
* designing tools for data retrieval templates or batch templates.
* defining reporting features.

#### Maintanance
* adding more file types and APIs for data retrieval (not JSON, .db, .csv, or .txt).
* 

## Goals
* Network infrastructure should use Chef Habitat and docker for deployment as well as a high authentication model that identifies sessions and applies this session to determine access to resource pools (for each app/service).
* Write Anna as a microservice infrastructure in nodejs, using postgreSQL, Vue.js, and python/js scripts. 
* Provide a data retrieval process that can automate virtually any accepted file or database into a common data build.
* Provide a data build process that can automate any common data build table into build views.
* Provide a way to connect build views to UI and services.
  1. Grids, or other user interface controls, defaulted by your organization, and customized by your users.
  2. APIs, microservices, communication channels between customers.
* Provide administration rules to control data builds and conversions, assign tasks and handle failures. Allow organization administrators to define these processes and who controls the ports
* Provide a method of saving, storing, restoring, encrypting, and compressing data that is cost effective and provides extensive usability.
* Development work should mostly consist of adding input file controls, reports, algorithms, and more involved in the business logic, rather than maintenance. We'd like to automate as much maintenance as possible on the overall system, while assigning developers to microservices to individually have authority over.

## Life Cycle
1. Data Retrieval-- A file is recieved by us through your company or customers.
2. Data Conversion-- Use a Conversion Layout with your file to map file data to a table.
3. Data Build-- Use one or many View Layouts to define view(s) for this new data.
4. ...
5. Profit!

#### Data Retrieval
No formatted files neccessary! As long as your files contain common encoding patterns, Anna will provide useful templating tools to help automate your data retrieval tasks.
