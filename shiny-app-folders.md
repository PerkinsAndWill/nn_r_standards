# Notes

-   Download a [sample folder here.](https://nn-r-resources.s3.us-west-2.amazonaws.com/sample-shiny-app-project-folder.zip) Note that it must be unzipped/extracted.
-   We recommend all Shiny apps use the multi-file configuration (e.g., ui.R, server.R, and global.R), as opposed to the one file option.
-   Please add subfolders to any of the folders laid out below as makes sense based on the complexity of your project. For example, if you have data over the course of multiple time periods, e.g., 2019 and 2020, it might make sense to have 2019 and 2020 subfolders.
-   If your Shiny application is a subfolder of a larger project that includes more than just a Shiny application, please refer back to the [generic project folder template](https://github.com/PerkinsAndWill/nn_r_standards/blob/main/generic-project-folders.md).
-   There are some additional hidden files (.git, .gitignore) that will appear when you initiate a Git repository within the project folder. For some quick instructions on how to initiate a Git version control repository within your R project, refer to [this page and select the tutorial that best matches your situation.](https://happygitwithr.com/usage-intro.html)

# Files

-   **ui.R**: User interface definition

-   **server.R**: Server code for application, where interaction with user inputs is happening.

-   **global.R**: Pre-launch set up for your application. Objects you create here will be accessible in both the server.R and the ui.R files.

-   **README.md**: This is a [markdown](https://rmarkdown.rstudio.com/articles_intro.html) file where you can describe the project in detail and include any information someone looking at this project later (including your future self) might need to know. If your project has a GitHub repository, this file will show up as HTML on the home page of the repository.

-   **\<YOUR-PROJECT\>.Rproj**: We recommend using an R Project so that all of your file paths will be relative to the parent directory of the project.

    -   *Important -- If your Shiny application is a sub-component of a larger project, it is still helpful to have an additional R Project file just for the Shiny application, so that you can operate from the same environment the Shiny application will be, rooted in the parent directory of the application (dictated by the parent directory of the above files.*

# Folders

-   **data/**: folder for storing data, with sub-folders as needed. Some examples of typical sub-folders below:

    -   **original/**: folder to store original/unmodified versions of input data associated with your project

        -   **shapefiles/**: optional folder for storing ESRI shapefiles (with have multiple files associated with a single geometric layer)

    -   **interim/**: folder to store modified versions of input data associated with your project (optional)

    -   **output/:** folder to store output data associated with your project (optional)

-   **functions/**: A folder for storing functions used inside your Shiny application. It is recommended to use functions where possible, both to simplify your server code and to more easily re-use functions for other projects.
