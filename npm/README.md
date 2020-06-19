# NPM
*node package manager*

### 
`npm init -y` accepts all the defaults  


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

* `npm install` : also

#### specific versions
*
`npm install <PACKAGE_NAME>@<VERSION>`  
<ins>Example</ins>:   
`npm install lodash@1.1.1`

### update a package 
`npm update lodash@1.1.1`

### install a package globally
`npm update -g lodash`

## list packages

`npm ls `
`npm list --depth 0`
#### Removing packages
`npm remove <PACKAGE_NAME>`

#### searching packages
`npm seatch <PACKAGE_NAME>`
### versions
* in the package.json  
`^` => install the lastest minor version  
`~` => install the latest patch version  
`*` => install the absolute latest version  

## Scripts

## Publishing packages
#### first, log to npm
**`npm login`**

**`npm publish --access public`**

### unpublishing a package
**`npm unpubish`**

#### display the current user 
**`npm whomai`**