# depser-demo

## Init

From mam root:

* `mkdir -p acme/depser && cd acme/depser`
* `Add .gitignore`
* `git submodule add --depth 100 https://github.com/zerkalica/yuf.git .ci/yuf`
* `.ci/yuf/depser/depser init`
* `mkdir -p app && echo '$acme_depser_app $mol_page' > app/app.view.tree`
* `git add .ci app && git commit -m 'updated deps`

## Add extra deps

Example:

* `.ci/yuf/depser/depser add "https://github.com/hyoo-ru/mam_hyoo.git" "hyoo"`
* `.ci/yuf/depser/depser add "https://github.com/hyoo-ru/about.hyoo.ru.git" "hyoo-about"`

## Build

From acme/depser directory:

* `.ci/yuf/depser/depser build`

Build in `./app/-`

## Update and fix deps

From acme/depser directory:

* `.ci/yuf/depser/depser update`
* `git add .`
* `git commit -m "updated deps"`
