# DFD Dictionary 

This file holds all definitions about the DFD Diagram.

## External Entities
* Fossology: External repository that holds information about source code, such as vulnerabilities... It returns information in SPDX format. 

## Internal Entities
* Corporate Developer: This is one of the company's asset. The Corpoerate Developer is the entry point of external software into the company.
* Corporate Manager: Manages the project, and its information.

## Data Flow
* File: Piece of source code.
* Package: Collection of files.
* File SHA1: Encription code of a file.
* File SHA1 Response: "yes" or "no". It is based on the existence of information about the file on the database.
* File Information: Information about the source code, such as vulnerabilities .
* File Information Request: Request for information about some piece of software.
* File Information Response: Contains information about the source code file.
* Project Information Request: Request for information about the project, such as vulnerabilities, status and etc.
* Project Information Response: Information about projects, such as vulnerabilities, status and etc.

## Data Store
* SPDX DB: Database that holds information about files (piece of source code), such as vulnerabilities.

## Processes
* Managing Code: Process of storing information about new source code, such as vulnerabilities, licenses.
* Managing Project Information: Supply project information of source code, such as vulnerabilities, licenses and etc. 
