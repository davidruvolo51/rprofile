# rprofile

This repo contains the `.Rprofile` and `.lintr` files that I often use across various projects. This configuration is optimized for R and vscode setups, but it can be used in other situations. If you `renv`, make sure the file is sourced last.

R Setup in vscode

- Radian: https://github.com/randy3k/radian
- Language Server: https://github.com/REditorSupport/languageserver

## Functions

There are two functions that I often use: `clear` (removes all objects in the environment) and `library2` (quietly loads packages).

```r
# clear: clear the active terminal
clear()

# rm2: removes everything in the current session except `clear`, `library2`, and `rm2`
rm2()

# library2: quietly load packages by default
library2("tidyverse")

```
