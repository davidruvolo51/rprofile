# rprofile

This repo contains the Rprofile file that I often use across various projects. This configuration is optimized for R and vscode setups, but it can be used in other situations. If you `renv`, make sure the file is sourced last.

R Setup in vscode

- Radian: https://github.com/randy3k/radian
- Language Server: https://github.com/REditorSupport/languageserver

## Functions

There are two functions that I often use: `clear` (removes all objects in the environment) and `library2` (quietly loads packages).

```r
# clear removes all objects except `clear` and `library2`
clear()

# use library2 to quietly load packages
library2("tidyverse")
```
