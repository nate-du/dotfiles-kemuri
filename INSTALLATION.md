# Ansible Installation

1. Install packages.
> sudo pacman -S git python ansible

2. Clone this repo into home directory.
#### HTTPS
> git clone https://github.com/nate-du/dotfiles.git
#### SSH 
> git clone git@github.com:nate-du/dotfiles.git

> cd dotfiles/ansible

3. Install AUR helper from ansible-galaxy. Used to install packages from AUR
(AUR helper defined in requirements.yml)

```
ansible-galaxy install -r requirements.yml
```

4. Run ansible. 
> ansible-playbook main.yml -K

5. Apply dotfiles using stow
> cd dotfiles

> stow btop fastfetch fish kitty spicetify vesktop vscode

6. Manually move remaining dots
* limine
* ly
* monketype
* noctalia (v4) - copy files to /.config/noctalia

