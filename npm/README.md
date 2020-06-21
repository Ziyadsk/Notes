# NPM
*node package manager*

### Create a new node app
* create a new package.json
> package.json is the configuration file for your node app  

**`npm init`** will prompt you for the informations of the app  
**`npm init -y`** accepts all the defaults without prompting


### Configs
#### Set/change the default configs
`npm set --init-author-name "<NAME>" `


#### Get the default configs
`npm get --init-author-name`

#### Delete some configs
`npm config delete --init-author-name`


### Installing packages
`npm install <PACKAGE_NAME>`

* add the `--save` flag to add the package to the current projects package.json as a dependency
* **`-g`** flag is used to install a package globally<br><br>
<ins>Example</ins>  
**`npm update -g lodash`**

* **`npm install`** also install dependecies if you modify the package.json directly

#### specific versions
* to install the exact version separate the package name and the version with an `@` symbol  
**`npm install <PACKAGE_NAME>@<VERSION>`**   
<ins>Example</ins>:   
`npm install lodash@1.1.1`

### Update a package 
`npm update lodash@1.1.1` 

### Update your app
`npm version <TYPE>`
<ins>Examples:</ins>  
`npm version major`  
`npm version minor`  
`npm version patch`  

## list packages

`npm ls `
`npm list --depth 0`
#### Removing packages
`npm remove <PACKAGE_NAME>`
* **`-g`** flag is used to remove a package globally

#### searching packages
`npm seatch <PACKAGE_NAME>`
### versions
* in the package.json  

`^<VERSION>` => install the lastest minor version  
`~<VERSION>`  => install the latest patch version  
`*`  => install the absolute latest version  
`<VERSION>`  => matches the exatcs version

npm version
### Scripts

## Publishing packages
#### First, log to npm
**`npm login`**
#### and then publish  
**`npm publish --access public`**

### unpublishing a package
**`npm unpubish`**

#### display the current user 
**`npm whomai`**

### Package.json 
bin   
scripts  
browser  
main   
man  