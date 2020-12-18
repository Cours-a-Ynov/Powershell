# Les Conditions
Vos scripts doivent souvent prendre des décisions et exécuter une logique différente en fonction de ces décisions.
C’est ce qu’on appelle une exécution conditionnelle.
Vous avez une instruction ou une valeur à évaluer, et vous exécutez une autre section de code en fonction de cette évaluation.
C’est là précisément qu’intervient l’instruction if.
L’instruction if vous permet de spécifier une action non seulement lorsque l’instruction est $true, mais également quand elle est $false. C’est ici qu’intervient l’instruction else.

En informatique, une instruction conditionnelle, (aussi appelé expression conditionnelle), est une fonction d'un langage de programmation, qui effectue différents calculs ou actions, en fonction de l'évaluation d'une condition booléenne, à savoir vraie ou fausse

Les blocs de conditions sont formés comme ceci

```
if (Condition){
intruction 1
} else {
instruction par défaut 
}
```

C'est à dire si la condition est respectée, le programme va exécuter l'instruction 1 sinon l'instruction par défaut.

Il existe aussi cette syntaxe

```
if (Condition){
intruction 1
} else if  {
instruction 2
} else if {
instruction 3
} else {
instruction par défaut 
}
```

On peut obtenir plus d'informations en tapant la commande suivante

help about_if

L’imbrication de conditions multiples est parfois difficile à établir et vous pourrez alors recourir à la directive “switch” (similaire au “select case” en vbscript) permettant de tester plusieurs cas de figure. Sa structure est la suivante :

```
switch (test ou évaluation de valeur) {
valeur1 { code à exécuter si test est égal à valeur1;break }
valeur2 { code à exécuter si test est égal à valeur2;break }
valeur3 { code à exécuter si test est égal à valeur3;break }

default { code à exécuter si test est égal à aucune des autres valeurs }
}
```

[Retour au sommaire](https://github.com/Malo44490/Powershell/blob/main/README.md#sommaire)
