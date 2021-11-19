# TP numéro 4

## Objectif:

Comprendre et utiliser les variables dans Ansible


## Besoin:

- Créer les répertoires *group_vars* et *hosts_vars*
- Créer le fichier *front* dans *group_vars* contenant `middleware: nginx`
- Créer le fichier *back* dans *group_vars* contenant `middleware: mariadb`
- Créer le fichier *server-4.scc-edu* dans *hosts_vars* contenant `middleware: aucun`
- Exécuter une tâche ad-hoc (module debug et var) pour afficher le contenu de la variable *middleware*
- Créer un fichier *server-1.scc-edu* dans *hosts_vars* contenant `middleware: nginx+`
- Exécuter une tâche ad-hoc (module debug et var) pour afficher le contenu de la variable *middleware*
- Exécuter une tâche ad-hoc (module debug et var) pour afficher le contenu de la variable *middleware* en ajoutant une **extra_var** `middleware=override`
