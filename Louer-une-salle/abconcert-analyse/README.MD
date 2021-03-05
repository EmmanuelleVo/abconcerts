# Page louer une salle

## Quick scan

|     | Description                                                                                     | Pondération | Score     |
| --- | ----------------------------------------------------------------------------------------------- | ----------- | --------- |
| 1   | Les titres de pages sont-ils significatifs?                                                     | 1           | 1         |
| 2   | La langue des pages est-elle correctement indiquée?                                             | 2           | 2         |
| 3   | Le focus est-il visible lors de la tabulation?                                                  | 2           | 0         |
| 4   | Le site est-il entièrement utilisable au clavier ?                                              | 3           | 0         |
| 5   | Est-il possible d’arrêter les animations?                                                       | 2           | /         |
| 6   | La différence entre les liens et le simple texte est-elle visuellement claire?                  | 1           | 0         |
| 7   | Les intitulés des liens sont-ils significatifs?                                                 | 2           | 0         |
| 8   | Toutes les images ont-elles une alternative textuelle?                                          | 2           | 2         |
| 9   | Les vidéos sont-elles sous-titrées?                                                             | 3           | /         |
| 10  | Le contraste entre le texte et l’arrière-plan est-il suffisant?                                 | 3           | 0         |
| 11  | Les titres sont-ils codés au moyen des balises HTML adéquates?                                  | 2           | 0         |
| 12  | Les listes sont-elles codées au moyen des balises HTML adéquates?                               | 1           | 1         |
| 13  | Les champs de formulaire sont-ils reliés à leur label?                                          | 2           | 0         |
| 14  | Une aide textuelle est-elle présente lorsque la validation d’un formulaire détecte des erreurs? | 2           | 2         |
| 15  | Le code source est-il valide?                                                                   | 1           | 0         |
|     |                                                                                                 |             | Total: 13 |

Le score est de 13/29, soit 44% de réussite.


1. Oui : "Louer une salle | Ancienne Belgique - Site Officiel",
2. Oui : <html lang="fr">,
3. Non : pas dans le menu de navigation,
4. Non : pas dans le menu de navigation,
5. / : il n'y a pas d'animation,
6. Non : "politique de confidentialité" dans le footer,
7. Non : pas dans le menu de navigation ("Mon AB" = Se connecter),
8. Oui : mais certaines ne sont pas significatives,

   ![Alt erreur](./img/alt-non-significatif.png)
   ![Alt correction](./img/alt-corr.png)
9. / : il n'y a pas de vidéos,
10. Non : pas dans le footer ni certains labels du formulaire,
11. Non : un titre est codé sous forme de label, et et beaucoup de sections n'ont pas de heading,
    ![Label erreur et correction](./img/label.png)
12. Oui,
13. Non : pas dans le footer,
14. Oui : quand le champ est obligatoire et que l'adresse mail doit être valide,
15. Non : pas du tout.

## HTML validator

![TotalValidator](./img/validator.png)
![w3-Validator](./img/validator-w3.png)

## Outline

Il manque notamment un titre (qui est originellement associé à un label)
![Headers Structure](./img/headers-original.png)

Correction :
![Headers Structure](./img/headers-corr.png)


Outline original :
![HTML5 Outline](./img/outline-error.png)

Correction :
![HTML5 Outline corr](./img/outline-corr.png)

## Rapport de contraste

![Contrast](./img/contrast-error.png)

Form :

- Labels
- Messages d'erreur

Footer

- La phrase "accéder directement à",
- Liens vers les conditions de vente ect.

## Microdata

![Microdata1](./img/microdata1.png)
![Microdata2](./img/microdata2.png)

## Carbon Calculator

La page "Louer une salle" d'ABConcert n'est pas du tout écologique comparée à la page d'accueil ou à la page d'un concert. En effet, il est plus "sale" que 94% des pages de sites web et la page produit 5.19 CO2 à chaque fois qu'un utilisateur visite cette page.
![Carbon Calculator](./img/carbon.png)

## GTMetrix

![GTMetrix1](./img/GT.png)
![GTMetrix2](./img/Metrix.png)
Il faudrait redimensionner l'image (Plus l'image a une haute résolution, plus son poids est lourd)
![Problème 1](./img/image-size.png)
Il faudrait compresser les images, ce qui réduirait la taille du fichier de l'image pour une meilleure performance
![Problème 2](./img/encode-image.png)
Il faudrait réduire la taille totale des requêtes de la page en minimisant la taille des ressources (compresser le HTML, CSS et JS)
![Problème 3](./img/network-payload.png)
Il faudrait que les données su site soient stockées dans le cache. Les données statiques (logos,...) pourraient être stockées pendant un an et le reste pendant un mois.
![Problème 4](./img/cache.png)


## Responsive

La page est tout à fait responsive

![Ordinateur-screenshot](./img/ordinateur.png)
![smartphone-screenshot](./img/smartphone.png)




## Refonte
   - Contraste des labels et messages d'erreur
   - Outline/headers : ajouts de titre, sections,nav, correction (label -> h2)
   - Ajout du FAQ dans le menu
   - Alt non significatifs
   - MonAB non significatif -> se connecter + bouton
   - Microdata
   - Newsletter : ajout d'un label
