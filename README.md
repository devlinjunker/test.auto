# Auto Versioning

Testing auto versioning with `npm install -D auto`

https://intuit.github.io/auto/pages/getting-started.html


GH_TOKEN added from github with repo/package permissions

## Labels created on Github

 - major
 - minor 
 - patch 
 - release 
 - internal
 - documentation


## Use

`npm run version` to update the version by a patch version number (i.e. 0.0.x), this will stop once the package is updated and not commited (after bump of version)
	- use this after each build

`./node_modules/.bin/auto changelog` generates the updated changelog based on commit messages and then creates a git commit on current branch

`./node_modules/.bin/auto release` pushes the current version number as a tag to github with the changelog


## Notes

 - You must not merge two PRs at once or you will botch one of the releases.


## Skip-Release label
https://intuit.github.io/auto/pages/quick-merge.html#with-skip-releaseo  
https://intuit.github.io/auto/pages/getting-started.html#enabling-skip-release-label  

 - skip-release label requires setup
 - allows merging multiple PRs quickly as it does not generate a new build/release

