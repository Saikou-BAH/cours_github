# Linux essentiel pour un data engineer débutant

## 1. Naviguer

Le but est simple : savoir où je suis, voir ce qu’il y a dans le dossier, entrer dans un dossier ou revenir en arrière.

### Commandes utiles

```bash
pwd -> Permet de savoir là où je suis
ls -> Permet de lister le contenu du dossier
ls -a -> Permet aussi de voir les fichers cachés ( par exemple .git)
ls -l -> Permet de voir le contenu avec plus de details
ls -la -> Une combinaise des deux précédentes commandes
cd nom_du_dossier -> Permet d'entrer dans le dossier nom_dossier
cd .. -> Permet de faire un seul pas en arriere
cd ~ -> Permet de revenir au dossier personnel
cd / -> Permet de revenir à la racine
cd - -> Permet de revenir au dossier précédent
```



## 2. Dossiers et fichiers

Le but ici est simple : savoir créer des dossiers, créer des fichiers, copier, déplacer, renommer et supprimer.

### Commandes utiles

```bash
mkdir projet -> Permet de créer un dossier appelé projet
mkdir -p data/raw/csv -> Permet de créer toute une arborescence d'un seul coup
touch fichier.txt -> Permet de créer un fichier vide
cp fichier.txt copie.txt -> Permet de copier un fichier
cp -r dossier dossier_copie -> Permet de copier un dossier avec tout ce qu'il y a dedans
mv ancien.txt nouveau.txt -> Permet de renommer un fichier ou un dossier
mv fichier.txt archives/ -> Permet de déplacer un fichier dans un autre dossier
rm fichier.txt -> Permet de supprimer un fichier
rm -r dossier -> Permet de supprimer un dossier avec tout son contenu
rm *.txt -> Permet de supprimer tous les fichiers qui finissent par .txt
rmdir dossier_vide -> Permet de supprimer un dossier vide
```

### A retenir

cp -> Permet de copier
mv -> Permet de déplacer ou renommer
rm -> Permet de supprimer
rmdir -> Permet de supprimer seulement un dossier vide



## 3. Lire un fichier

Le but ici est simple : savoir lire un fichier rapidement, voir le début, voir la fin et lire plus proprement un gros fichier.

### Commandes utiles

```bash
cat fichier.txt -> Permet d'afficher tout le contenu du fichier
cat -n fichier.txt -> Permet d'afficher le contenu du fichier avec les numéros de ligne
head fichier.txt -> Permet de voir le début du fichier
head -n 5 fichier.txt -> Permet de voir les 5 premières lignes du fichier
tail fichier.txt -> Permet de voir la fin du fichier
tail -n 5 fichier.txt -> Permet de voir les 5 dernières lignes du fichier
less fichier.txt -> Permet de lire un gros fichier plus proprement dans le terminal
more fichier.txt -> Permet de lire un fichier page par page
q -> Permet de quitter less ou more
```

### A retenir

cat -> Permet de lire tout le contenu d'un petit fichier
head -> Permet de voir le début d'un fichier
tail -> Permet de voir la fin d'un fichier
less -> Permet de lire un gros fichier plus proprement
more -> Permet de lire un fichier page par page
q -> Permet de quitter less ou more



## 3. Lire un fichier

Le but ici est simple : savoir lire un fichier rapidement, voir le début, voir la fin et lire plus proprement un gros fichier.

### Commandes utiles

```bash
cat fichier.txt -> Permet d'afficher tout le contenu du fichier
cat -n fichier.txt -> Permet d'afficher le contenu du fichier avec les numéros de ligne
head fichier.txt -> Permet de voir le début du fichier
head -n 5 fichier.txt -> Permet de voir les 5 premières lignes du fichier
tail fichier.txt -> Permet de voir la fin du fichier
tail -n 5 fichier.txt -> Permet de voir les 5 dernières lignes du fichier
less fichier.txt -> Permet de lire un gros fichier plus proprement dans le terminal
more fichier.txt -> Permet de lire un fichier page par page
q -> Permet de quitter less ou more
```

### A retenir

cat -> Permet de lire tout le contenu d'un petit fichier
head -> Permet de voir le début d'un fichier
tail -> Permet de voir la fin d'un fichier
less -> Permet de lire un gros fichier plus proprement
more -> Permet de lire un fichier page par page
q -> Permet de quitter less ou more


## 4. Chercher et filtrer

Le but ici est simple : savoir chercher un mot dans un fichier, trouver un fichier, compter et filtrer un résultat.

### Commandes utiles

```bash
grep "mot" fichier.txt -> Permet de chercher un mot dans un fichier
grep -i "mot" fichier.txt -> Permet de chercher un mot sans faire attention aux majuscules et minuscules
grep -n "mot" fichier.txt -> Permet de chercher un mot avec le numéro de ligne
grep -v "mot" fichier.txt -> Permet d'afficher les lignes qui ne contiennent pas le mot
grep -c "mot" fichier.txt -> Permet de compter combien de lignes contiennent le mot
find . -name "notes.txt" -> Permet de trouver un fichier précis à partir du dossier courant
find . -name "*.txt" -> Permet de trouver tous les fichiers qui finissent par .txt
wc -l fichier.txt -> Permet de compter le nombre de lignes
wc -w fichier.txt -> Permet de compter le nombre de mots
wc -c fichier.txt -> Permet de compter le nombre de caractères
cat fichier.txt | grep "mot" -> Permet de filtrer le contenu d'un fichier avec un pipe
ls > liste.txt -> Permet d'écrire le résultat dans un fichier en écrasant l'ancien contenu
ls >> liste.txt -> Permet d'ajouter le résultat à la fin du fichier
```

### A retenir

grep -> Permet de chercher du texte dans un fichier
find -> Permet de chercher un fichier ou un dossier
wc -> Permet de compter
| -> Permet d'envoyer le résultat d'une commande vers une autre
> -> Permet d'écrire en écrasant
>> -> Permet d'ajouter à la fin