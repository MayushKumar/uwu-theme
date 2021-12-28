# UwU Theme
An awesome dark color scheme for emacs.

## Screenshot
![UwU emacs theme](https://github.com/kborling/uwu.el/blob/main/uwu.png)

## Try It

1. Clone repo `git clone https://github.com/kborling/uwu.el.git` in directory of your choosing.
2. Type `M-x load-file` and choose the `uwu-theme.el` file.
3. Type `M-x enable-theme` and choose `uwu`.

## Installation

### Manual
1. Clone repo `git clone https://github.com/kborling/uwu.el.git` in directory of your choosing. 
2. Add the following code in your emacs config file:
   ```elisp
   (add-to-list 'custom-theme-load-path "~/.emacs.d/themes") ;;; Make a themes directory and add uwu.el to it

   (load-theme 'uwu t t)
   (enable-theme 'uwu)
   ```
   
### Using Straight.el
1. [Install Straight.el](https://github.com/raxod502/straight.el#getting-started)
2. Add the following code in your emacs config file:
   ```elisp
   (straight-use-package
      '(uwu-theme :host github :repo "kborling/uwu.el"))
   (require 'uwu-theme)
   (load-theme 'uwu t)
   ```
   
### Using Doom Emacs Packages.el
1. Add the following code in your `~/.doom.d/packages.el` file:
   ```elisp
   (package! uwu-theme
      :recipe (:host github :repo "kborling/uwu.el"))
   ```
2. Add the following code in your `~/.doom.d/config.el` file:
   ```elisp
   (require 'uwu-theme)
   (load-theme 'uwu t)
   ```
   
### Using spacemacs packages
1. Append the following inside your `~/.config/spacemacs` `dotspacemacs-additional-packages` variable.
    ```elisp
    (uwu-theme :location (recipe :fetcher github :repo "kborling/uwu.el"))
    ```
2. prepend `'uwu'` to the theme variable:
   ```elisp
      dotspacemacs-themes '(uwu)
   ```
   
## Acknowledgments
- Inspiration and Color Scheme based on https://github.com/Mangeshrex/uwu.vim
