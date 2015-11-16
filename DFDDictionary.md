# DFD Dictionary 

This file holds all definitions about the DFD Diagram.

## External Entities
* National Vulnerability Database: National Instute of Standards and Technology's NVDB is a repository maintained by the United States government, containingof standards based vulnerability management data.
* OSS Community: Represents open source repositories to which source code taken from the community is re-published.

## Internal Entities
* Corporate Developer: Builds the project, and report to the corporate managers.
* Version Control System: Source code repository.
* Corporate Manager: Manages the project, and its information.  

## Data Flow
* File/Package: Single file or collection of files (package).
* License Info: List of licenses of the file or package.
* Package Query: The current name of the package.
* CPE Information: Standard name of a package.
* File SHA1 Request: Encription code of a file.
* File SHA1 Response: "Yes" or "No". It is based on the existence of information about the file on the database.
* File License, CPE and CVE Info: Information about the source code, such as standard name, licenses, vulnerabilities, etc.
* Project Info Request: it requests information about the project, such as what open source software is being utilized on the project and what are licenses and vulnerabilities.
* Project Info: It contains information about projects, such as what open source software is being utilized on the project and what are licenses and vulnerabilities.
* Project Policy Comparison: It is a report originated from the comparison between the project information and the corporate policy.
* CPE Info: It is the new version of the XML that holds Common Platform Enumeration information.
* CPE Information Request: It requests a new version of the XML that holds Common Platform Enumeration information.
* CPE Information Response: It is the response containing the new version of the XML that holds Common Platform Enumeration information.
* Project Info Response/Policy Info Request: It sends the information about the open source package, and it requests policy info.
* Policy Info Response: It is the result of the compliance check performed on the Manage Policy Information process.
* Policy Info Request: It requests information about the company's policy about open source software.
* Policy Info Response: It is the the company's policy about open source software.
* CVE Information: This is the response to the CVE Information Request, returns the CVE information itself.
* Project File/Info Request: A request by the corporate manager; For the files of the project, or project info
* Package File/Info Response: A repsonse to the corporate managers; contains whatever was requested.
* File / Package: The files or packages of the project
* Project File: The file of the project
* License and Vulrability Info: Information returned from FOSSology and NIST National Vulnerability Database regarding the licenese and CVEs.
* CVE Info Request: This is the request sent to the National Vulrability Database for Common Vulnrabilities and Exposures
* CPE and CVE Info: This is the response sent from the National Vulrability Database for Common Platform Enumeration and Common Vulnrabilities and Exposures.
* Request OSS License Compliance: This is the request sent to developers to check what open source softwares need to be sent back to the community. 
* OSS License Compliance Response: This is the developer's response about the status of the OSS License Compliance. This response update managers about the status of the task.
* Modified Package: The open source software taken from the community with modifications made by developers to fit into the organization's need.


## Data Stores
* NIST CPE Information: It holds the standard (global) names for packages of softwares. It is a XML file that is held locally. It is downloaded from the National Vulnerability Database website.
* License DB: Software Package Data Exchange Database that holds information about open source software, such as standard name, licenses, vulnerabilities, etc.
* Policy DB: Data store that holds the company's policy information.

## Processes
* Manage Code Streams: Process of gathering information about open source software, such as licenses and vulnerabilities. This process also persists the information into the company database.
* License Scanner: Process of gathering information about licenses for specific files or packages.
* Manage Project Information: Provides information about a specified open source code. 
* Manage CPE Information (Daily Job): This process is responsible to update the NIST CPE Information data store by downloading the latest version from the National Vulnerability Database.
* Manage Policy Information: This process takes the information about the open source software and check to see if there is a match between the package licenses and vulnerabilities with the company's policy.
* Version Control System: The company's internal source code repository. This process helps manage commits and changes to the codebase.
* Licesnse Scanner: This process provides information about what licenses are in packages for the open source software used.
* Vulnerability Lookup: This process is responsible for using CPE information to query the National Vulnerability Database for CVE information
* Contribute Code to Community: This process is for contributing any code back to the OS community that was taken from it by the developers.
* OSS License Compliance: This process defines formal request/response for software license compliance between managers and developers.
