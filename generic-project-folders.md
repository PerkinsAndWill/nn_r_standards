# Notes

-   If your project contains one or more Shiny applications, please refer to the [Shiny application project template](<https://github.com/PerkinsAndWill/nn_r_standards/blob/main/shiny-app-folders.md>) for those sub-folders. If your project is *only* a shiny application, you can proceed directly to that template.

# Files

-   **README.md**: This is a [markdown](<https://rmarkdown.rstudio.com/articles_intro.html>) file where you can describe the project in detail and include any information someone looking at this project later (including your future self) might need to know. If your project has a GitHub repository, this file will show up as HTML on the home page of the repository.
-   **\<YOUR-PROJECT\>.Rproj**: We recommend using an R Project so that all of your file paths will be relative to the parent directory of the project.

# Folders

-   **data/**: folder for storing data, with sub-folders as needed. Some examples of typical sub-folders below:

    -   **original/**: folder to store original/unmodified versions of input data associated with your project

        -   **shapefiles/**: optional folder for storing ESRI shapefiles (with have multiple files associated with a single geometric layer)

    -   **interim/**: folder to store modified versions of input data associated with your project (optional)

    -   **output/:** folder to store output data associated with your project (optional)

-   **scripts/**: A folder for storing the scripts used for your project. Please create sub-folders within this folder as necessary for the complexity of your project. Typical sub-folders I use include the following:

    -   **data-processing/**

    -   **analysis/**

    -   **model-testing/**

    -   **plot-generation/**

-   **functions/**: A folder for storing functions used for your project. It is recommended to use functions where possible, both to simplify your script code and to more easily re-use functions for other projects. As above, please create sub-folders within this folder as necessary for the complexity of your project.

-   **\<your-shiny-app\>/**: A folder for storing the application code and associated data (and R Project file) for a Shiny application. If you have more than one Shiny application associated with your project, please create additional parent folders and R Projects for each application.
