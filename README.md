# Dotfiles

Just a repo with my dotfiles. 

If you want to use it, clone the repo into your root folder `~/` and place this script in `.bash_profile`:

```shell
# Load the shell dotfiles, and then some:
# * ~/.path can be used to extend `$PATH`.
# * ~/.extra can be used for other settings you don’t want to commit.
for file in ~/.dotfiles/.{path,bash_prompt,exports,aliases,functions,extra}; do
  [ -r "$file" ] && source "$file"
done
unset file
```
