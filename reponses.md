question 1 : si vous essayez de supprimer la branche actuelle, Git refuse l'opération et affiche un message d'erreur car C'est parce que vous ne pouvez pas supprimer la branche sur laquelle vous êtes actuellement.

question 2 :Utilisez la commande suivante :
git diff main feature-1
Cela affichera toutes les différences entre les deux branches.

question 3 : Observez l’historique des commits dans feature-rebase :
$ git log --oneline --graph --all
* f915680 (HEAD -> feature-rebase) Ajout de la deucieme ligne du fichier feature.txt
* 4ebfe44 Ajout du fichier feature.txt
* aecd625 (main) Modification du README sur le main
* b8fce8c Ajour d'un fichier sur le main
* 548b3dc Modification sur le README sur le main
*   ef61d82 Resolution du conflit en gardant les deux versions
|\
| * d96428c (conflit-test) Modification du README sur conflit-test
* | 84a37f0 Modification du README sur main
|/
* 5d95fff Ajout du fichier notes.txt dans la branche dev
| * 6eb84f4 (feature-1) Aout d'une modification dans feature-1
|/
* dd6334e (feature-2) Premier commit : creation du README

