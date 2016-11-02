# Use npm modules' cli commands without doing `npm install -g`

# Why?

Now instead of doing `npm install -g gulp` or similar and then having mismatches between your global gulp version and your package's locally installed gulp you can just run your usual `npm install` and can still do `gulp` as usual. 

# Usage

### `zgen`

```sh
zgen load nikvdp-node-modules-plugin
```

### `antigen`

```sh
antigen bundle nikvdp/node-modules-plugin
```

# How does it work?

This is a small hook that adds your `node_modules/.bin` directory to your shell's PATH variable whenever you're in a directory that has a `node_modules` folder or a `packages.json` file. 

# Credits

This is just a lightly edited combination of [add-zsh-hook](https://github.com/zsh-users/zsh/blob/master/Functions/Misc/add-zsh-hook) and [npm_chpwd_hook](https://gist.github.com/puffnfresh/4151775)
