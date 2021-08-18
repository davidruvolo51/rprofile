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
rm2(except = c("someObjectName", "anotherObjectName"))

# library2: quietly load packages by default
library2("tidyverse")

```

## Install

You can use this setup in other projects. There are few things you will need to change before you get started. First, clone this repository and change the remotes. 

```zsh
git clone https://github.com/davidruvolo51/rprofile/
git remotes origin <new-remote>
```

Second, rename &mdash; or remove &mdash; the vscode workspace file

```zsh
mv rprofile.code-workspace <new-filename>
```

Lastly, restore the renv and update packages accordingly.

```r
renv::restore()
renv::update()
```
