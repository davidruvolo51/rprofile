#' @title Clear Environment
#' @name clear
#' @description Force remove all objects from the current environment
#' @noRd
clear <- function() {
    rm(list = setdiff(ls(envir = .GlobalEnv), "clear"), envir = .GlobalEnv)
}

#' @title Quietly Import Package
#' @name import
#' @param pkg the name of the package
#' @noRd
import <- function(pkg) {
    
}


# start renv: make sure this is always last!
source("renv/activate.R")
