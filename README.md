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

Au lieu d'apporter des modifications au répertoire sur la branche `master` par défaut, nous allons travailler sur une nouvelle branche pour effectuer ces modifications.

- Pour créer une branche, utilisez la commande suivante depuis le repertoire `test-pull-request-2022`

```shell
$ git checkout -b <new-branch-name> 
```
- Où `<new-branch-name>` est le nom de la branche que nous allons appeler : `pull-request-test-<votre_utilisateur> `


