# bash-qcs

**Unacknowledge the user when typing wrong commands.**

This is a fork of [hkbakke](https://github.com/hkbakke)'s [bash-insulter](https://github.com/hkbakke/bash-insulter) whith less insults and more ceratis.

Graphics made with [Google Images](https://images.google.com/search?q=quien+chota+sos), [Pinetools](https://pinetools.com/pixelate-effect-image), [Imagemagick](https://imagemagick.org/index.php), [Gimp](https://www.gimp.org/), and [img2xterm](https://github.com/denilsonsa/img2xterm)

## Compatibility

* Bash v4 and newer
* Zsh
* 256-colour terminals

## Installation

    # Method 1 - know what you are doing
    git clone https://github.com/juanpsm/bash-qcs.git bash-qcs
    sudo cp bash-qcs/src/bash.command-not-found /etc/

    # Method 2 - I don't care, unacknowledge me!
    sudo wget -O /etc/bash.command-not-found https://raw.githubusercontent.com/juanpsm/bash-qcs/master/src/bash.command-not-found

Then source the file automatically for new logins by adding the following to `/etc/bash.bashrc` or any of the other locations where you can configure your shell automatically during login:
```
if [ -f /etc/bash.command-not-found ]; then
    . /etc/bash.command-not-found
fi
```
Login again and type some invalid commands for the effects to be visible.

Note: You will have to add the script to `.zshrc` if you are using `zsh`

# Thanks

* 