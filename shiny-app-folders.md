# Notes

- We recommend all Shiny apps use the multi-file configuration (e.g., ui.R, server.R, and global.R), as opposed to the one file option.

# Required

## Files
- **ui.R**: User interface definition
- **server.R**: Server code for application, where interaction with user inputs is happening. 
- **global.R**: Pre-launch set up for your application. Objects you create here will be accessible in both the server.R and the ui.R files. 

## Folders

- **data/**: folder for storing data, with sub-folders as needed. Some examples of typical sub-folders below:
 - **shapefiles/**
- **functions/**: A folder for storing functions used inside your Shiny application. It is recommended to use functions where possible, both to simplify your server code and to more easily re-use functions for other projects.

# Optional

