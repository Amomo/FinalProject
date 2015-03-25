# The Unix System & User Information Analyzer

`The Unix System & User Information Analyzer` is our final project on CS312A Introduction to UNIX Operating System

We want to provide a easy way for users and admins to get the useful info from the complex system tools!

## File structure

```
|__project's root
  |__draftScripts - temperary scripts
  |__textVersion  - text version scripts
  |__webVersion   - web version scripts
```
## Usage

extract the tarball or clone the project from github, get into the directory

and run `webVersion/run.sh` or `textVersion/run.sh`

the result will be placed unber that two directories' sub-directory - `results`

If you have root permission, it will scan all the user info, or it will just scan your user info.

You can use this tool with crontab, so that the result will be updated automatically!

For example, run the web version every hour :
`00  * * * * /home/root/TUSUIA/webVersion/run.sh`

## Requirement

To analysis user info, you will need `finger` tool

To analysis network info, you will need `vnstat` tool

Most of the remaining tools we used are built-in tool.
