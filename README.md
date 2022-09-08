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
One of the biggest reasons to use a package manager, is their powerful dependency management. Instead of manually having to make sure that you get all dependencies whenever you set up a project on a new computer, npm automatically installs everything for you. But how can npm know exactly what your project needs? Meet the dependencies section of your package.json file.
In this section, packages your project requires are stored using the following format: 
`"dependencies": {
  "package-name": "version",
  "express": "4.14.0"
}
`
* ## Manage npm Dependencies By Understanding Semantic Versioning
`Versions` of the npm packages in the dependencies section of your package.json file follow what’s called **Semantic Versioning (SemVer)**, an _industry standard for software versioning aiming to make it easier to manage dependencies_. Libraries, frameworks or other tools published on npm should use SemVer in order to clearly communicate what kind of changes projects can expect if they update.

Knowing SemVer can be **<u>useful when you develop software that uses external dependencies</u>** (which you almost always do). One day, your understanding of these numbers will save you from accidentally introducing breaking changes to your project without understanding why things that worked yesterday suddenly don’t work today. This is how Semantic Versioning works according to the official website:
`"package": "MAJOR.MINOR.PATCH"`
### The **MAJOR** version should increment when you make incompatible API changes. 
### The **MINOR** version should increment when you add functionality in a backwards-compatible manner. 
### The **PATCH** version should increment when you make backwards-compatible bug fixes. 
### This means that PATCHes are bug fixes and MINORs add new features but neither of them break what worked before. 
### Finally, _MAJORs add changes that won’t work with earlier versions._

* ## Use the Tilde-Character to Always Use the Latest Patch Version of a Dependency
To allow an npm dependency to update to the latest PATCH version, you can prefix the dependency’s version with the **tilde (~) character**. Here's an example of how to allow updates to any 1.3.x version.
`"package": "~1.3.8"`

* ##Use the Caret-Character to Use the Latest Minor Version of a Dependency
Similar to how the tilde we learned about in the last challenge allows npm to install the latest PATCH for a dependency, the **caret (^) allows npm to install future updates as well. _The difference is that the caret will allow both MINOR updates and PATCHes.**_

Your current version of @freecodecamp/example should be "~1.2.13" which allows npm to install to the latest 1.2.x version. If you were to use the caret (^) as a version prefix instead, npm would be allowed to update to any 1.x.x version.
`"package": "^1.3.8"`

* ## Remove a Package from Your Dependencies
You have now tested a few ways you can manage dependencies of your project by using the package.json's dependencies section. You have also included external packages by adding them to the file and even told npm what types of versions you want, by using special characters such as the tilde or the caret.

But what if you want to remove an external package that you no longer need? You might already have guessed it, just remove the corresponding key-value pair for that package from your dependencies.

This same method applies to removing other fields in your package.json as well.
 