
# Composer Version Test

Just a simple dummy project that doesn't do anything but 
allows you to test the ways to require a package using tags versions, constraints and stabilities


## Installation

Use composer to download the project in you project

```bash
  composer require --dev fgalvao/version-test
```
or in your `composer.json`

```json
 "require-dev" : {
     "fgalvao/version-test" : xxxx
 }
```
##Docs  
Not sure how, check out the composer version documentation https://getcomposer.org/doc/articles/versions.md

Don't want to install this package in you local, test on-line here [semver.mwl.be](https://semver.mwl.be/?package=fgalvao/version-test&constraint=dev-main&stability=stable)
    
## Usage/Examples

Just change the version you want to download in you `composer.json`

```json
{
  "prefer-stable": true|false,
  "minimum-stability": "dev|alpha|beta|rc|stable",

  "require-dev": {
      "fgalvao/version-test" : "1.1", OR
      "fgalvao/version-test" : "^1.1@beta", OR 
      "fgalvao/version-test" : "^1.1@rc"
  }
}
```

and check the version on you console
```batch
composer show | grep fgalvao/version-test
```

you can see all the available versions using:
```batch
composer show -a fgalvao/version-test 
```

  