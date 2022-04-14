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

- En ligne de commande réduire sa qualité de 50% et nommer cette nouvelle
image image_converted.jpg
- [ ] Rendu : Un pdf contenant toutes les lignes de commandes que vous avez tapées
et l’image finale.
> Aide : Vous devrez télécharger un paquet magick vous permettant de convertir
l’image