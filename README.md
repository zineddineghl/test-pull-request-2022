# test-pull-request-2022

Référentiel pour tester la pull request du cours [Introduction à la gestion de version à l’aide de git](https://juanluck.github.io/Introduction-GIT/).

## Instructions pour faire une pull request 

### 1. Faire un fork du référentiel actuel 

- Accéder à ce référentiel https://github.com/juanluck/test-pull-request-2022
- Cliquez sur `fork` en haut à droite de github. 

![Fork](./images/fork.png)

- Le fork vous permet de copier ce référentiel sur votre compte github. Désormais, vous pouvez travailler avec cette copie du référentiel original. Cela va vous permetre d'expérimenter librement et faire des modifications sans affecter le projet d'origine. 

- Voir qu'après le `fork`, vous avez une copie du référentiel dans votre propre espace `https://github.com/<votre_utilisateur>/test-pull-request-2022`

- Créez un nouveau répertoire sur votre machine local (que vous pouvez appeler par exemple `tp4`) et clonez le référentiel depuis votre compte :

```shell
$ ls
tp1 tp2 tp3 
$ mkdir tp4
$ ls
tp1 tp2 tp3 tp4
$ cd tp4
$ git clone git@github.com:<votre_utilisateur>/test-pull-request-2022.git
...
$ cd test-pull-request-2022
```

- Voila, vous avez déjà une copie locale sur votre machine. **Attention !!**, n'apportez pas encore de modifications. Pour effectuer de tels changements, nous allons travailler avec une branche dans la section suivante. 

### 2. Création d'une branche thématique 

Au lieu d'apporter des modifications au répertoire sur la branche `main` par défaut, nous allons travailler sur une nouvelle branche pour effectuer ces modifications.

- Pour créer une branche, utilisez la commande suivante depuis le repertoire `test-pull-request-2022` :

```shell
$ git checkout -b <new-branch-name> 
```
- Où `<new-branch-name>` est le nom de la branche que nous allons appeler : `pull-request-test-<votre_utilisateur>`

- Pour vérifier que l'espace de travail est bien sur la nouvelle branche (et non sur la branche `main`) tapez :

```shell
$ git branch
  main
* pull-request-test-<votre_utilisateur>
```
- L'étoile * indique la branche sur laquelle vous travaillez. Désormais les modifications n'affectent que cette branche. Assurez-vous que cette branche est bien `pull-request-test-<votre_utilisateur>`

- La branche créée appartient à votre répertoire local, mais le répertoire distant n'en a pas encore connaissance. Pour synchroniser les changements entre le répertoire local et distant, écrivez la commande : 

```shell
$ git push origin pull-request-test-<votre_utilisateur>
```



