# Ember CLI Helper

[![Gitter chat](https://badges.gitter.im/alexlafroscia/atom-ember-cli-helper.png)](https://gitter.im/alexlafroscia/atom-ember-cli-helper)

[ember-cli](https://github.com/stefanpenner/ember-cli) integration in Atom.

![ember cli helper](http://f.cl.ly/items/0C1A110I3w2G2P0k0Z1T/Screen%20Shot%202015-03-22%20at%205.34.37%20PM.png)

## Commands

| Command  | Description                                                    |
| :--      | :--                                                            |
| Server   | Runs `ember server` in the root folder of the project.         |
| Test     | Runs `ember test` in the root folder of the project            |
| Generate | Opens the panel to run a generator                             |
| Exit     | Stops a currently running process                              |
| Minimize | Show and hide the output panel, without hiding everything else |
| Close    | Hide the entire panel                                          |

## Generators

Running the generators through Atom is really easy.  When you first open the panel, it will bring up a list of file types to generate.  This list is based on the output of `ember g --help`, and therefore should include all future blueprints as well as those added by addons automatically. Once you select a type, you'll be prompted to enter a name, and the output will appear in orange in the bottom panel.

## Help! It's broken!

That might be the case! But first, check if specifying the path to the Ember and NPM packages fixes your problems.  It probably, hopefully will.  If it doesn't, please file an issue so I can try fixing it!

## Settings

| Setting | Purpose | Default Value |
| :---    | :---    | :---          |
| Generate Coffeescript     | Have all of the generators make CoffeeScript files instead of Javascript | `false` |
| Path To Ember Executable  | Point the CLI helper to the Ember executable on your computer | `/usr/local/bin/ember` |
| Path To `node` Executable | Point the CLI helper to the `node` executable on your computer | `/usr/local/bin/node` |

## Todo List

- [x] Open `ember-cli-helper` automatically if the package uses the Ember CLI
- [ ] Differentiate a task's button from the others when it is active
- [ ] Use the editor's theme to get colors for success and error in the command output
- [ ] Give some sort of visual feedback about the running command when the panel is minimized
- [x] Include a panel for running the file generators

## Troubleshooting

Some users have experienced problems running the commands when they openning their project through the `File > Open` menu.  If this happens to you, try opening the project from the command line with the `atom` command see if that fixes the issue.


***

**Special thanks** to [@nickclaw](https://github.com/nickclaw/) and his
[atom-grunt-runner](https://github.com/nickclaw/atom-grunt-runner)
package, which was my inspiration for building this and a big help in putting it
together.
