# wre-static-pages-semantic-ui

# About 

site styles are located here

`/semantic/src/site/globals/site.overrides`

Perhaps we could organization components into individual files i.e. footer.variables and footer.overrides, but I put them all in one for now.


## Semantic was setup using the following procedure

1. Install Gulp using NPM (if NPM isn’t already on your system, we recommended adding it via the Nodejs installer)

`> npm install gulp -g`

2. Run npm init to create a `package.json` file (just hit enter to accept the default install options).

`> npm init`

3. Now we’re ready to install semantic-ui. Use the default options so that it installs in the `semantic/` folder.

`> npm install semantic-ui -D`

4. Next we need to modify our semantic.json file to adding an `autoInstall: true` setting. This will allow Netlify to build your site without getting stuck during the interactive semantic-ui installation. Just open your semantic.json file and change the `autoInstall` setting from `false` to `true`.

`"autoInstall": true,`

5. Next, create a `.gitignore` file with the following exclusions. (We don’t need to commit these directories to git since they will be generated during the build anyway.)

```
semantic/node_modules/
node_modules/
semantic/dist/
````

