# todo.txt-mitf

This is an add-on for [`todo.txt-cli`](https://github.com/ginatrapani/todo.txt-cli/), and more specifically an extension to the [MIT add-on](https://github.com/codybuell/mit).

This add-on allows the user to generate MIT TODOs for certain day in the future.
Assuming today's YYYY-MM-DD date is 2016-01-15, then the command `todo.sh mitf 10d "Foo @bar +baz"` would result in running the MIT command `todo.sh mit 2016.01.25 "Foo @bar +baz"`.

## Sample commands:

```plain
$ date -Idate
2016-11-13

$ todo.sh mitf 3d "Foo @bar +baz"
85 2016-11-13 {2016.11.16} Foo @bar +baz
TODO: 85 added.

$ todo.sh mitf 1w "Foo @bar +baz"
86 2016-11-13 {2016.11.20} Foo @bar +baz
TODO: 86 added.

$ todo.sh mitf 2m "Foo @bar +baz"
87 2016-11-13 {2017.01.13} Foo @bar +baz
TODO: 87 added.
```

## Installation

Clone this repo and copy the [`mitf`](mitf) file into your add-on folder;
ordinarily the folder name will be `~/.todo.actions.d` (see [Installing Addons](https://github.com/ginatrapani/todo.txt-cli/wiki/Creating-and-Installing-Add-ons) for more information).
