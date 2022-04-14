# Challenges

## Challenge 1
- Mettre à jour ubuntu :

```bash
 sudo apt update && sudo apt upgrade -y && sudo apt dist-upgrade -y
 ```

- En ligne de commande, télécharger l’image : https://promo-159.codeur.online/photo/surprise.jpg et la nommer image.jpg

```bash
wget https://promo-159.codeur.online/photo/surprise.jpg
mv surprise.jpg image.jpg
```

ou :

```bash
wget --output-document=image.jpg https://promo-159.codeur.online/photo/surprise.jpg
```

- En ligne de commande réduire sa qualité de 50% et nommer cette nouvelle image image_converted.jpg

```bash 
sudo apt install imagemagick
convert image.jpg -quality 50% image_converted.jpg
```

- [X] Rendu : Un pdf contenant toutes les lignes de commandes que vous avez tapées et l’image finale.
> Aide : Vous devrez télécharger un paquet magick vous permettant de convertir l’image

### Résultats

- L'image renommée : 

![image.jpg](image.jpg)

- L'image avec réduction de qualité de 50% : 

![image_converted.jpg](image_converted.jpg)



----



## Challenge 2 

- Créer un dossier « Challenges »

``` bash
mkdir Challenges
```

- Aller dans ce dossier

``` bash
cd Challenges
```

- Créer un fichier texte « hello_world »

```bash 
> hello_world
```

- Avec la commande `echo` , écrire 3 lignes dans ce fichier :
-- Nom Prénom
-- Date du jour
-- Hello World !

``` bash
echo "Hareche Amine"
echo "14/04/2022"
echo "Hello world !"
```

- Pour affiché le fichier et son contenu

```
cat hello_world
```

- Mettre ce fichier en lecture seule ( qu’il soit impossible d’écrire à nouveau
dedans )

```bash 
chmod a=r hello_world
```


- [X] Rendu : toutes les lignes de commandes que vous avez tapées



-----



# Challenge 3
- Dans le dossier « Challenges » créer un script qui prend en paramètre un chiffre et qui calcule sa table de multiplication (de 0 à 10)

``` bash
touch multiplication
```

- Donner les droits sur le fichier : 

``` bash 
chmod +x multiplication
```

- modifier le fichier : 

``` bash 
nano multiplication
```

- Créer le script :

``` bash
#!/bin/bash
echo "Entrez un chiffre :"
read -r chiffre
echo 'Votre chiffre est :' $chiffre

for (( i=0 ; i<10 ; i++ ))
 do
  echo $((chiffre*i))
 done
 ```
 
 - Lancer le script : 

``` bash
./multiplication
```

- [X] Rendu : un fichier markdown contenant  contenant votre script
