# Backend Challenges boilerplate - package.json
[![Run on Repl.it](https://repl.it/badge/github/freeCodeCamp/boilerplate-npm)](https://repl.it/github/freeCodeCamp/boilerplate-np**ss**m)  

* ## Add Keywords to Your package.json
### The `keywords` field is where you can describe your project using related keywords. Here's an example:
### ``"keywords": [ "descriptive", "related", "words" ],``
* ## Add a License to Your package.json
### The `license` field is where you inform users of what they are allowed to do with your project.
Some common licenses for open source projects include MIT and BSD. License information is not required, and copyright laws in most countries will give you ownership of what you create by default. However, it’s always a good practice to explicitly state what users can and can’t do. Here's an example of the license field:
### `"license": "MIT",`
* ## Add a Version to Your package.json
### A version is one of the required fields of your package.json file. This field describes the current version of your project. Here's an example:
### `"version": "1.2.0",`
* ## Expand Your Project with External Packages from npm
### One of the biggest reasons to use a package manager, is their powerful dependency management. Instead of manually having to make sure that you get all dependencies whenever you set up a project on a new computer, npm automatically installs everything for you. But how can npm know exactly what your project needs? Meet the dependencies section of your package.json file.
### In this section, packages your project requires are stored using the following format: 
`"dependencies": {
  "package-name": "version",
  "express": "4.14.0"
}
`
 