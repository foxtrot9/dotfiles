# Steps:

1. Install brew first. See https://brew.sh/ .

2. Download this repo as zip because SSH is not setup.

https://github.com/foxtrot9/dotfiles/archive/refs/heads/master.zip

3. Install brew dependencies.

```
brew bundle install
```

4. Configure ZSH
```
cp dotfiles/zshrc .zshrc
```

5. Install oh-my-zsh : https://github.com/ohmyzsh/ohmyzsh?tab=readme-ov-file#basic-installation

6. Apply iTerm config.

Go to Preferences > General > Preferences and select "Load preferences from a custom folder or URL" and
use `$HOME/dotfiles/iTerm`.

Don't save local settings to this file.

Set "Save changes" to "Manually". 

7. Configure SSH

Get SSH config and keys from current device and copy them to new device.

```
ssh-add ~/.ssh/$KEY
```

## TODO

- [ ] Upgrade dotbot and use it for installing configuration. Update README.md with instructions.

- [ ] Add ssh key to apple keychain so that ssh-add command doesn't need to be run at every login.

