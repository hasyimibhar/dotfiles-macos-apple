Based on https://drewdevault.com/2019/12/30/dotfiles.html

## Steps

1. Install developer tools:
   ```sh
   sudo xcode-select --switch path/to/Xcode.app
   ```
   
2. Install oh-my-zsh:
   ```sh
   sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
   ```

3. Clone this repo into `$HOME`:
   ```sh
   cd $HOME
   git clone git@github.com:hasyimibhar/dotfiles-macos-apple
   mv dotfiles-macos-apple/.* .
   rm -rf dotfiles-macos-apple
   ```

4. Install `brew`:
   ```sh
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```
   
5. Install `wezterm`:
   ```sh
   brew install --cask wezterm
   ```
   
6. Install `skhd`:
   ```sh
   brew install koekeishiya/formulae/skhd
   skhd --start-service
   ```
   
7. Install `yabai` and [disable SIP](https://github.com/koekeishiya/yabai/wiki/Disabling-System-Integrity-Protection):
   ```sh
   brew install koekeishiya/formulae/yabai
   yabai --start-service
   ```

8. Install `neovim`:
   ```sh
   brew install neovim ripgrep
   ```

9. Install [Logseq](https://logseq.com/downloads) and [Google Drive Desktop](https://www.google.com/drive/download/).
