# depser-demo

## Init

From mam root:

* `mkdir depser && cd depser`
* `Add .gitignore`
* `git submodule add --depth 100 https://github.com/zerkalica/yuf.git .ci/yuf`
* `.ci/yuf/depser/depser init`
* `mkdir -p app && echo '$depser_app $mol_page' > app/app.view.tree`
* `git add .ci app && git commit -m 'updated deps`

## Build

* `.ci/yuf/depser/depser build`

Build in `./app/-`

## Update and fix deps

* `.ci/yuf/depser/depser update`
* `git add .`
* `git commit -m "updated deps"`
