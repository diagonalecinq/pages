# Diagonale

Site statique construit avec Jekyll et le thème `minima`.

## Structure du projet

- `pages/_config.yml` : configuration Jekyll
- `pages/_posts/` : billets du blog
- `pages/blog.md` : page du blog
- `pages/manifeste.md` : page dédiée au manifeste

## Prérequis

Pour lancer le site en local, il faut installer l'environnement Ruby :

- Ruby
- Bundler
- Jekyll

Sous Windows, le plus simple est d'utiliser RubyInstaller avec Devkit :

- Site : `https://rubyinstaller.org/`
- Installer une version stable récente de Ruby avec Devkit
- Pendant l'installation, ajouter Ruby au `PATH`

## Vérifier l'installation

Ouvrir un nouveau terminal PowerShell puis vérifier :

```powershell
ruby -v
bundle -v
```

Si `bundle` n'est pas disponible :

```powershell
gem install bundler
```

## Dépendances du projet

Le projet contient un `Gemfile` minimal pour exécuter le site localement avec Bundler.

## Installation des dépendances

Depuis le dossier `pages` :

```powershell
bundle install
```

Lors de la première installation, Bundler téléchargera Jekyll, `minima`, `jekyll-feed` et les dépendances Ruby nécessaires.

## Lancer le site en local

Depuis le dossier `pages` :

```powershell
bundle exec jekyll serve
```

Puis ouvrir dans le navigateur :

```text
http://127.0.0.1:4000
```

## Rechargement automatique

Pour activer le rechargement automatique du navigateur :

```powershell
bundle exec jekyll serve --livereload
```

## Commandes utiles

Installer Bundler :

```powershell
gem install bundler
```

Installer Jekyll globalement si nécessaire :

```powershell
gem install jekyll
```

Vérifier les versions :

```powershell
ruby -v
bundle -v
jekyll -v
```

## Remarques

- Les commandes doivent être lancées depuis `c:\Users\Diagonale\Documents\CODE\pages`
- Si `bundle` ou `jekyll` n'est pas reconnu, il faut vérifier que Ruby est bien installé et disponible dans le `PATH`
- Après installation de Ruby sous Windows, il est préférable d'ouvrir un nouveau terminal avant de retester les commandes