<div align="center">

[![](https://yt-embed.herokuapp.com/embed?v=g9_6KmiBISk)](https://www.youtube.com/watch?v=g9_6KmiBISk)

# Yarn Package Manager Crash Course

</div>

---

Yarn is a Javascript package manager created by facebook

Faster and more reliable than NPM

NPM is still the most popular package manager since it was the first one developed. still, yarn is gaining momentum

Yarn installs packages from the NPM registry so anything that you can install with NPM you can also install with the yarn as well

in `npm5` no need to use `--save` flag anymore

---

#### INSTALLATION

```sh
npm install --global yarn
```

#### GET VERSION

```sh
yarn -v (or --version)
```

#### GET HELP

```sh
yarn help
```

#### CREATE PACKAGE.JSON

```sh
yarn init
yarn init -y // Use defaults
```

#### SET DEFAULTS

```sh
yarn config set init-license ISC
```

#### GET DEFAULTS

```sh
yarn config get init-license
```

#### REMOVE DEFAULTS

```sh
yarn delete init-license
```

#### INSTALLING LOCAL PACKAGES

```sh
yarn add lodash
yarn add moment
```

#### INSTALL FROM PACKAGE.JSON

```sh
yarn install
```

#### REMOVING MODULES

```sh
yarn remove lodash
```

#### INSTALL CERTAIN VERSIONS

```sh
yarn add lodash@4.17.3
```

#### FIND OUTDATED VERSIONS

```sh
yarn outdated lodash
yarn outdated
```

#### UPGRADE

```sh
yarn upgrade lodash
yarn upgrade
```

#### INSTALL GLOBAL MODULE 

global must be put right after yarn while npm is flexible

```sh
npm install -g nodemon    (or)    npm install nodemon -g
``` 
```sh
yarn global add nodemon
```

#### FIND ROOT FOLDER

```sh
yarn global bin
```

#### REMOVE GLOBAL PACKAGES

```sh
yarn global remove nodemon
```

#### LISTING PACKAGES

```sh
yarn list
yarn list --depth=0
yarn list --depth=1
yarn list --pattern gulp
```

#### INSTALLING AS DEV DEPENDENCY

```sh
yarn add gulp -D    (or)    yarn add gulp --dev
```

#### REMOVE DEV DEPENDENCY

```sh
yarn remove gulp
```
when we ran `yarn init` it created this `yarn.lock` file and basically this is used for to have consistent installs across a machine so it holds exactly which versions of the dependencies that were installed along with the repo link

#### VERIFY THAT VERSIONS MATCH LOCK FILE

```sh
yarn check
```

#### CREATE YARN.LOCK FILE

```sh
yarn import
```

#### ADD SCRIPT

```json
{
    "scripts": {
        "dev": "nodemon index.js"
    },
}
```

#### RUN SCRIPT

```sh
yarn run dev
````

#### GET LICENSES

```sh
yarn license
```

#### CREATE GZIP ARCHIVE OF DEPENDENCIES

```sh
yarn pack
yarn pack mydep
```

#### LIST GLOBAL CACHE PACKAGES

```sh
yarn cache list
yarn cache list --pattern lodash
```
