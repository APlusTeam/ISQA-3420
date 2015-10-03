# DFD Dictionary 

This file holds all definitions about the DFD Diagram.

## External Entities
* National Vulnerability Database: 

## Internal Entities
* Corporate Developer: This is one of the company's asset. The Corporate Developer is the entry point of external software to the company.
* Corporate Manager: Manages the project, and its information.  

## Data Flow
* File: Piece of source code.
* Package: Collection of files.
* File/Package: File or Package
* License Info: List of licenses of the file or package.
* Package Query: The current name of the package.
* CPE Information: Standard name of a package.
* File SHA1 Request: Encription code of a file.
* File SHA1 Response: "Yes" or "No". It is based on the existence of information about the file on the database.
* File License and CPE Information: Information about the source code, such as standard name, licenses, vulnerabilities, etc.
* Project Info Request: it requests information about the project, such as what open source software is being utilized on the project and what are licenses and vulnerabilities.
* Project Info Response: It contains information about projects, such as what open source software is being utilized on the project and what are licenses and vulnerabilities.
* File Info Request: It requests information about a piece of software.
* File Info Response: it contains information about the source code, such as standard name, licenses, vulnerabilities, etc.
* CPE Info: It is the new version of the XML that holds CPE information.
* CPE Request: It requests a new version of the XML that holds CPE information.
* CPE Response: It is the response containing the new version of the XML that holds CPE information.

## Data Store
* NIST CPE Information: It holds the standard (global) names for packages of softwares. It is a XML file that is held locally. It is downloaded from the National Vulnerability Database website.
* SPDX DB: Database that holds information about open source software, such as standard name, licenses, vulnerabilities, etc.

## Processes
* Manage Code Streams: Process of gathering information about open source software, such as licenses and vulnerabilities. This process also persists the information into the company database.
* FOSSology: Process of gathering information about licenses for specific files or packages.
* Manage Project Information: Provides information about a specified open source code. 
* Manage CPE Information (Daily Job): This process is responsible to update the NIST CPE Information data store by downloading the latest version from the National Vulnerability Database.
