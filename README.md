# Winget-exclude-packages-from-upgrade
Just add ID package in $Package = @(.....) and start the script


## Francais :
Le script utilise une comparaison de fichiers car il est difficile de trier les ID dans un fichier de sortie de la commande "winget upgrade > fichier".
Il compare donc les résultats du fichier à un fichier export de tous les paquets (commande proposée par winget) 
qui est plus facile à manipuler et donc plus facile pour exclure les paquets qu'on ne souhaite pas mettre à jour. 
La comparaison entre les deux garde seulement les résultats identiques, 
donc seulement les paquets qui peuvent être mis à jour avec une exclusion pour ceux qu'on ne souhaite pas mettre à jour.

## Anglais : 
The script uses a file comparison because it is difficult to sort the IDs in an output file of the "winget upgrade > file" command.
It therefore compares the results of the file to an exported file of all packages (a command proposed by winget)
which is easier to manipulate and therefore easier to exclude packages that are not desired to be installed.
The comparison between the two only keeps identical results, so only the packages that can be updated with exclusions.
