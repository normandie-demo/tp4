# Correction TP 4


## Création des dossiers et des fichiers

```Shell
mkdir {host_vars,group_vars}

vi group_vars/front

vi group_vars/back

vi host_vars/server-4.scc-edu
```

## Exécuter une tâche ad-hoc (module debug et var) pour afficher le contenu de la variable *middleware*

```Shell
ansible -i inventory '*' -m debug -a 'var=middleware'
```

## Création du fichier pour server-1

```Shell
vi host_vars/server-1.scc-edu
```

## Exécuter une tâche ad-hoc (module debug et var) pour afficher le contenu de la variable *middleware*

```Shell
ansible -i inventory 'front' -m debug -a 'var=middleware'
```

## Exécuter une tâche ad-hoc (module debug et var) pour afficher le contenu de la variable *middleware* en ajoutant une **extra_var** `middleware=override`
```Shell
ansible -i inventory 'front' -m debug -a 'var=middleware' -e middleware=override
```








