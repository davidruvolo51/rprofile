#' ////////////////////////////////////////////////////////////////////////////
#' FILE: .Rprofile
#' AUTHOR: David Ruvolo
#' CREATED: 2021-07-29
#' MODIFIED: 2021-07-29
#' PURPOSE: my Rprofile
#' STATUS: working; ongoing
#' PACKAGES: NA
#' COMMENTS: optimized for radian, vscode R
#' ////////////////////////////////////////////////////////////////////////////

# set options
options(

    # options: shiny
    shiny.port = 8000,
    shiny.launch.browser = FALSE,

    # options: radian
    radian.prompt = "\033[0;34m>\033[0m ",

    # options: vscode R
    vsc.use_httpgd = TRUE,
    vsc.helpPanel = "Beside",
    vsc.viewer = "Beside",
    vsc.browser = "Beside",
    vsc.show_object_size = FALSE,

    # options: languageserver
    languageserver.formatting_style = function(options) {
        styler::tidyverse_style(start_comments_with_one_space = TRUE)
    }
)


#' @title Clear Environment
#' @name clear
#' @description Force remove all objects from the current environment
#' @noRd
clear <- function() {
    ignore <- c("clear", "library2")
    rm(list = setdiff(ls(envir = .GlobalEnv), ignore), envir = .GlobalEnv)
}

#' @title Quietly Load Package
#' @name library2
#' @description suppress messages when loading a package
#' @param pkg the name of the package
#' @noRd
library2 <- function(pkg) {
    suppressPackageStartupMessages(library(pkg, character.only = TRUE))
}

# start renv: make sure this is always last!
source("renv/activate.R")