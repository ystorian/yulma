# yulma
A modern [Zola](https://www.getzola.org/) theme made with [Bulma](https://bulma.io/) for [Ystorian](https://ystorian.com)


## Bulma
Add the Bulma repo in `vendor/bulma`, and keep only the `sass` subdirectory.
```shell
git submodule add git@github.com:jgthms/bulma.git vendor/bulma
cd vendor/bulma
git sparse-checkout init --cone
git sparse-checkout set sass
```

## Directories

### `/sass`
Contains the Sass files to be compiled.

Non-Sass files will be ignored.

The directory structure of the sass folder will be preserved when copying over the compiled files; for example, a file at sass/something/site.scss will be compiled to public/something/site.css.


### `/static`
Contains any kind of file.
All the files/directories in the static directory will be copied as-is to the output directory.


### `/vendor/bulma`
Bulma submodule.

### `/vendor/bulma/sass`
Bulma sass files, referenced in `/sass/css/yulma.scss`.
