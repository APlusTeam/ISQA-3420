# DFD Dictionary 

This file holds all definitions about the DFD Diagram.

## External Entities
Fossology: External repository that holds information about source code, such as vulnerabilities, ... . It returns information in SPDX format. 

## Internal Entities
Corporate Developer: company's asset. The developer is the entrance point of external software to the company.

Corporate Manager: manages the projects.

## Data Flow
File: piece of source code.
Package: collection of files.
File SHA1: encription code of a file.
File SHA1 Response: "yes" or "no". It is based on the existence of information about the file on the database.
File Information: information about the source code, such as vulnerabilities ... .
File Information Request: request for information about some piece of software.
File Information Response: contains information about the source code file.
Project Information Request: request for information about the project, such as vulnerabilities, status and etc.
Project Information Response: information about projects, such as vulnerabilities, status and etc.

## Data Store
SPDX DB: database that holds information about files (piece of source code), such as vulnerabilities, ... .

## Processes
Managing Code: process of storing information about new source code, such as vulnerabilities, licenses.

Managing Project Information: suply project information of source code, such as vulnerabilities, licenses and etc. 
