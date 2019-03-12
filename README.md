# Angular-cli-redirect-script

Server configuration file to add to your project for URL rewrite to work fine in production

# How to use

- copy the file depending on your platform to the source root directory of your project (`<project_patch>/src/`)
    * `.htaccess` for apache
    * `web.config` for IIS
- open the file `angular.json` or `angular-cli.json` depending on the angular version (should be at the root of your project)
- add the script to the build assets like the favicon `favicon.ico` or the `assets` directory

For apache :

```json
"assets": [
    "src/favicon.ico",
    "src/assets",
    "src/.htaccess"
]
```

For IIS :

```json
"assets": [
    "src/favicon.ico",
    "src/assets",
    "src/web.config"
]
```