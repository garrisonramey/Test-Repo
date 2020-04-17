# Pelori Dataset Converter
## Team Information
### Group: 0452
### Members: Sahar Ali, Megha Desai, Collin Kemper, Garrison Ramey, Sonica Sahetiya, Sam Scheele
-------------------------------------------------------------------------------
## Release Notes

#### Version 1.0.0 <br>
#### New Software Features:
- Supports choosing a .dataset file or annotation directory as the source to be converted
- Supports choosing a destination path where the new annotations will be placed
- Allows file navigation of the machine on which the datasets exist
- Supports selection of multiple dataset formats to convert to
- Shows the progress of the conversion as it is happening
- Details of the conversion are displayed once the conversion has finished
- Metadata pertaining to specific datasets is displayed 

#### Bug Fixes Since Last Release:
- Added support for Windows
- Added a scroll view to the file navigation component
- Updated the user interface to be more user friendly
- Added dataset toolkit to support the conversion
- Added dataset reader to create and handle .dataset files

#### Known Bugs and Defects:<br>
The application currently sends requests to the Django local server at 127.0.0.1:8000. If you wish to manage datasets on a remote server, you will need to update the urls that exist in the following files with your server's address: <br>
- pelori-project/frontend/src/app/conversion.service.ts
- pelori-project/frontend/src/app/datasetinfo.service.ts
- pelori-project/frontend/src/app/file.service.ts

## Install Guide

#### Pre-requisites:
- Python3 (https://www.python.org/downloads/)
- Node.js (https://nodejs.org/en/download/)<br><br>
The application will work on the following operating systems:
- Linux
- Windows
- macOS

#### Dependent libraries that must be installed:
- Angular
Once Node.js is installed, you can install Angular by opening a terminal and running<br> `npm install -g @angular/cli`
- Django<br>
 `python3 -m pip install Django`

#### Installation:
1) Clone this repository
2) Extract files if you downloaded it as a ZIP file
3) You should have a directory structure similar to the figure below:<br>
 pelori-project<br>
    ├── backend<br>
    ├── frontend <br>
    ├── test<br>
4) Change your current working directory to <b>pelori-project/frontend</b>
5) In <b>pelori-project/fontend</b>, run the following command to install the necessary modules<br>
  `npm install`
6) You should now have all the necessary software to run the application, please see the <b>Run Instructions</b> on how to 
start the application
    
No specific directories are required after the software is built. However, this application depends on our client's dataset toolkit, so for it to function properly, you must request access to the toolkit by emailing a member of our group. To install the dataset toolkit, you must add it to your Python site-packages directory.
#### Run Instructions:
1) Open two separate terminal windows
2) In the first terminal window, change your current working directory to <b>pelori-project/backend</b> and run<br> `python3 manage.py runserver`
3) In the second terminal window, change your current working directory to <b>pelori-project/frontend</b> and run<br>
`ng serve`
4) Open your web browser and go to 127.0.0.1:4200 or localhost:4200 to use the application

#### Troubleshooting:
There may be issues when installing the necessary dependencies using `npm install`. If this happens, simply delete the "node_modules" folder and run `npm install` again to retrieve the dependencies defined in package.json
