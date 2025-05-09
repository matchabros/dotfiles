# My Dotfiles

> DO NOT USE THESE DOTFILES IN THIS STATE

## Update 2025-05-09

- This all needs updating

## To do

[ ] Find a way to get your current settings into this repo
[ ] Specific dotfiles for setting up your python environment
[ ] Specific dotfiles for setting up git, ssh, etc.
[ ] Dotfiles to download: Chrome, VSCode, iTerm, Notion
[ ] Dotfiles to create specific directories on my desktop

## How to use them

This is my repository for my dotfiles, as I am still on El Cap I finally decided it is time to switch to Sierra and in Sept/Oct to High Sierra (altho macOS Covefe would be a much more intriguing name). These dotfiles are heavily inspired by Mathias Bynens and Dries Vints, thus I am really grateful for their guidance. I highly encourage you to go through the files and decide on your own which parts you actually need.

## Fresh Install

Mostly, we should follow the instructions of Dries Vints.

1. Update macOS to the latest version with the App Store
2. Install Xcode from the App Store, open it and accept the license agreement
3. Install macOS Command Line Tools by running `xcode-select --install`
4. Copy public and private SSH keys to `~/.ssh` and make sure they're set to `600`
5. Clone this repo to `~/.dotfiles`

6. Append `/usr/local/bin/zsh` to the end of your `/etc/shells` file

>Note: point 6. can be done by going into `Terminal.app` typing `sudo nano /etc/shells` at the bottom of the list of available shells add `/usr/local/bin/zsh` press `ctrl+x` confirm changes.

7. Run `install.sh` to start the installation

## Now, if you have mackup ready (by that I mean you actually use it), follow these steps.

8. Make sure Dropbox is set up and synced
9. Restore preferences by running `mackup restore`
10. Restart your computer to finalize the process


> Note: you can use a different location than `~/.dotfiles` if you want. Just make sure you also update the reference in the `.zshrc` file.

Dries mentiones to keep you `.zshrc` file backed by `mackup`, therefore not be required to keep that particular file inside of this repo. I will make sure to do so.

> Thank you so very much Dries and Mathias!