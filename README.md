# tidybiobespoke
This package allows you to use your own tidy datasets to automatically generate an "Introduction to Tidyverse" presentation

# Installation
To install this package, run the following in your RStudio console -    
`devtools::install_github("BAREJAA/tidybiobespoke")`

# Run a bespoke presentation in the Tutorial pane of RStudio
Change your working directory to the one that contains the files you will need -  
`setwd(system.file("extdata", package = "tidybiobespoke"))`

The file `Tidybio functions.R` contains code for two funtions that allow you to generate .R files that contain the necessary meta data to run your presentation. After loading the `rstudioapi` package, run the code that creates the `make_metadata()` function (beginnining at line 3). Now run `make_metadata()` with the given (example) arguments. This will generate a new untitled .R file which you must save as `metadata.R` in the `inst/tutorials/lecture10_intro_to_select/code` folder.

Go to line 44 of `Tidybio functions.R` and run the code that creates the `bespoke()` function. Now run `bespoke()` with the given (example) arguments. This will generate a new untitled .R file which you must save as `bespoke.R` in the `inst/tutorials/lecture10_intro_to_select/code` folder.

Create an empty folder within the main `tidybiobespoke` folder called `inst`. Copy the `tutorials` folder (the folder + its contents) into `inst`. You should now have an `inst/tutorials` folder that has the same contents as `tutorials`.

Finally, run the following in your console -  
`learnr::run_tutorial("lecture10_intro_to_select", "tidybiobespoke")`

This will open the bespoke presentation in your browser. You will also now see this presentation in your Tutorial pane, which allows you to run the presentation within the RStudio environment.



