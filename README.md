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
