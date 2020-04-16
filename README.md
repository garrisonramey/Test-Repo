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
