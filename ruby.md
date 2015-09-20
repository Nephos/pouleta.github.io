<meta charset="utf-8" />

# Installer Ruby
**Installation d'un environnement de développement Ruby propre**

## Installations

### Rbenv

Rbenv permet de gérer son environnement de développement très simplement : version de ruby, gems, etc.

* L'installation peut se faire via son répo git : [rbenv sur github](https://github.com/sstephenson/rbenv)
* Ou alors via un gestionnaire de paquet (apt-get install rbenv, …)

### Ruby-build

Extension de rbenv, elle permet l'installation des versions de ruby (téléchargement, compilation, ...)

* L'installation peut se faire via son répo git : [ruby-build sur github](https://github.com/sstephenson/ruby-build)
* Ou alors via un gestionnaire de paquet (apt-get install ruby-build, …)

### Mise à jour du $PATH

Il faut ensuite mettre à jour son bashrc / zshrc / config

#### Bash, Zsh, …

```
export PATH="$HOME/.rbenv/bin:$PATH"
export PATH="$HOME/.rbenv/shims:$PATH"
rbenv rehash >/dev/null
```

#### Fish

```
set PATH $HOME/.rbenv/bin $PATH
set PATH $HOME/.rbenv/shims $PATH
rbenv rehash >/dev/null ^&1
```
