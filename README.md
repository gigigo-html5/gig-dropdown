# gig-dropdown
[Gigigo](http://www.gigigo.com/app/en/home) Gigigo Webcomponent to manage dropdowns

## Installation

Download node at [nodejs.org](http://nodejs.org) and install it, if you haven't already.

```sh
bower install gig-dropdown --save
```

## Run Demo

We use npm package [local-web-server](https://www.npmjs.com/package/local-web-server) to serve our files, but you are free to use whatever you want.

```sh
npm sun serve
```

## Develop / Contributions

All code changes must be done inside src/ folder and then run gulp release task to 'create' distribution.
Distribution files are the ones in the project root folder.

## Tests

```sh
npm install
npm test
```

## Other NPM Scripts

To check both our npm and bower dependencies we are using package [npm-check-updates](https://www.npmjs.com/package/npm-check-updates)

1. Check npm dependencies:

```sh
npm run check-npm-deps
```

2. Check bower dependencies

```sh
npm run check-bower-deps
```

3. Update all dependecies

```sh
npm run update-deps
```

## Release a new version

- copy everything to package root and change some paths on files
```
npm run release
```

- merge (ONLY) from develop to master
```
git merge --no-ff develop
```

- release (patch, minor or major) package and push changes to repo
```
npm run release:[version]
git push
```

## License

MIT
