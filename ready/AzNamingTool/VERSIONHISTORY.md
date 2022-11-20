﻿[Overview](./) | [Installation](INSTALLATION.md) | [Updating](UPDATING.md) | [Using the API](USINGTHEAPI.md) | [Version History](VERSIONHISTORY.md) | [FAQ](FAQ.md) | [Contributors](CONTRIBUTORS.md)

# Azure Naming Tool v2 - Version History

<img src="./wwwroot/images/AzureNamingToolLogo.png?raw=true" alt="Azure Naming Tool" title="Azure Naming Tool" height="150"/>

## Version 2.3.1 (current)

### Bug fixes
- Updated Configuration page to export Admin configuration, if selecteddocumentation
- Updated ResourceTypes.cs model to not require Short Name.

***

## Version 2.3.0
### Features
- Added Search functionality to Admin Log
- Added Search functionality to Generated Names Log
- Added caching throughout application for performance/optimization
- Added functionality to check for latest version. Admins will be prompted if the installed version is out of date.
- Added functionality to check for Resource Type and Location file versions. Admins will be prompted if the installed version is out of date.
- Added FAQ.md in GitHub
- Added CONTRIBUTORS.md in GitHub
- Added GitHub Action for deployment to Azure Web App
- Added "Deploy to Azure" options for installation

### Bug fixes
- Fixed grammar/formatting issues in GitHub documentation
- Updated resourcetypes.json with latest Azure resources
- Added information/update prompt to Configuration page if resaourcetypes.json contains types with duplicate short names
- Added option to enable/disbale Latest News feed on Home page
- Added option to exlcude Admin configuration from Global Backup functionality
- Updated API to handle resource types with duplicate names
- Added Admin Log and Generated Names log data to Global Configuration backup/restore functionality
- Updated Installation.md with new guidance

***

## Version 2.2.0
### Features
- Added VERSIONHISTORY.md file
- Added ability to exclude resource type component for resource types
- Added Latest Azure Naming Tool News feed to Home page (from twitter.com/azurenamingtool feed)
- Added Custom Component functionality
	- Updated Configuration page with new functionality
	- Updated Reference page to display custom components if present
	- Updated Generate page to display custom components if present
	- Updated API - RequestName function to accept Custom Components

### Bug fixes
- Added logic to prevent duplicate resource type short names
- Added notification to Configuration page for duplicate resource types short names to prompt for refresh
- Updated Refresh Resource Types utility to refresh short names by default
- Updated /repository/resourcetypes.json with new data
- Added enhanced Admin Log messaging
- Moved Admin Log link to top of navigation
- Added Resource Type to Generated Names Log
- Updated Configuration page button styling
- Updated Generate page component selection logic

***

## Version 2.1.0
### Features
- Updated RequestName API function to only require basic text for name generation. This simplifies name generation via the API.
- Created RequestNameWithComponents API function for legacy name generation
- Updated GitHub documentation to separate files
	- README.md - Overview of the Azure Naming Tool
	- INSTALLATION.md - Instructions for installing the Azure Naming Tool
	- UPDATING.md - Instructions for updating an installation
	- USINGTHEAPI.md - Instructions for integrating with the API

### Bug fixes
- Moved Admin Log Message and Generated Name logging to new LogHelper class
- Updated API documentation

***

## Version 2.0.0
- Initial release
