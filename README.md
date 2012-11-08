# Bash it

### forked from [revans/bash-it](https://github.com/revans/bash-it)
**Bash it** is a mash up of revan's own bash commands and scripts, other bash stuff he has found.
(And a shameless ripoff of [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh). :)
Includes autocompletion, themes, aliases, custom functions, a few stolen pieces from Steve Losh, and more.

## Envision Modifications
### envision branch
Created the envision template and theme (based off pete theme) to focus primarily on displaying git repository information as the existing themes and templates seemed to be heavily focused around ruby and other technologies which threw errors because the packages were not installed and they also cluttered up the prompt with unnecessary information. The colours have been adjusted to clearly highlight the current branch and branch status whilst making the other information more subtle in comparison.

### envision-clean branch
Includes all of the envision branch changes plus we also removed all of the plugins, aliases and completions that were irrelevant to our environment here at envision.  You probably don't want this branch as it's specific to our needs.

## Install

1. Check a clone of this repo: `git clone http://github.com/wwjamieson3/bash-it.git ~/.bash_it`
2. Checkout the branch you want to use `cd ~/.bash_it/ && git checkout envision`
3. Run `~/.bash_it/install.sh` (it automatically backs up your `~/.bash_profile`)
4. Install envision template `cp -f ~/.bash_it/template/envision.template.bash ~/.bash_profile`

## Help Screens

```
bash-it show aliases        # shows installed and available aliases
bash-it show completions    # shows installed and available completions
bash-it show plugins        # shows installed and available plugins
bash-it help aliases        # shows help for installed aliases
bash-it help completions    # shows help for installed completions
bash-it help plugins        # shows help for installed plugins
```

## Your Custom scripts, aliases, and functions

For custom scripts, and aliases, just create the following files (they'll be ignored by the git repo):

* `aliases/custom.aliases.bash`
* `lib/custom.bash`
* `plugins/custom.plugins.bash`

Anything in the custom directory will be ignored, with the exception of `custom/example.bash`.

