# ArcGIS Admin Toolkit

The ArcGIS admin toolkit contains a number of tools and scripts to administer ArcGIS Server and Desktop. The following tools are available:

#### Cache Map Service
Caches a map service by either creating a new cache from scratch using a configuration file or by updating an existing cache.

#### ArcGIS Server Availability
Checks ArcGIS server site and services and reports if site is down and/or particular service is down. This tool should be setup as an automated task on the server.

#### ArcGIS Server Permissions
Checks ArcGIS server service or folder for any permission changes. 

#### Action Windows Service
Restarts the windows service specified.
* Needs to be run as administrator.

#### Import ArcGIS Server Users
Imports a list of users provided in a CSV file to ArcGIS server, assigning to roles and setting default password.

#### Backup and Restore ArcGIS Server Site
* Restores an ArcGIS server site from a backup file.
* Creates a site if no site has been created, otherwise will overwrite previous site. 
* Restores the license.
* Need to include data in map service OR make sure referenced data is in same place.
* The arcgisserver directories need to be in the same file path on the restore server as the backup server.
* Does not include map caches
* Need to have ArcGIS for Server and ArcGIS web adaptor for IIS installed (if wanting to restore web adaptor).

#### Start or Stop GIS Services
Starts or stops GIS services. Can start/stop all GIS services for an ArcGIS server site or just the ones that are specified.

#### ArcGIS Server Stats
Generates a CSV file with statistics around how often services are being used and how well they are performing in the ArcGIS server site.

#### Map Service Test
Runs a configurable query against a map service and produces a report on draw times at specified scales.

#### Map Service Monitor
Checks a map service for instance usage and performance. This tool should be setup as an automated task on the server. 
* Needs to be run as administrator. 
* Need to install WMI python package.


## Features

* Automate the administration process.
* Maintain geodatabase performance.
* Setup map caching as a scheduled task.
* Monitor ArcGIS Server site.
* Backup and restore site configurations.
* Start or stop GIS services
* Get ArcGIS server performance statistics.


## Requirements

* Python for ArcGIS installed. Version required is specified in the comments section of each individual script.


## Installation Instructions

* Tools can be run from the operating system command prompt (stand-alone), in a Python IDE or as a geoprocessing script tool.
* Setup a script to run as a scheduled task
	* Fork and then clone the repository or download the .zip file. 
	* Edit the [batch file](/Examples) to be automated and change the parameters to suit your environment.
	* Open Windows Task Scheduler and setup a new basic task.
	* Set the task to execute the batch file at a specified time.


## Resources

* [LinkedIn](http://www.linkedin.com/in/sfweston)
* [GitHub](https://github.com/WestonSF)
* [Twitter](https://twitter.com/Westonelli)
* [Blog](http://westonelli.wordpress.com)
* [ArcGIS Blog](http://blogs.esri.com/esri/arcgis)
* [Python for ArcGIS](http://resources.arcgis.com/en/communities/python)


## Issues

Find a bug or want to request a new feature?  Please let me know by submitting an issue.


## Contributing

Anyone and everyone is welcome to contribute. 


## Licensing
Copyright 2015 - Shaun Weston

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.