<style>
  * {
    font-size: 20px;  
  }
  h1, h2 {
    color: #caad2a;
  }
  ul {
    list-style-type: square;
  }
</style>

# **Difficultés rencontrées et Solutions**
## **I. Version desktop**
- **Problème 1 :** La bordure bleue qui apparait au-dessus des liens de navigations au passage du curseur déplaçait tous les éléments de la page vers le bas. 

- **Solution 1 :** J'ai défini une bordure de couleur blanche (la couleur de fond) de même épaiseur aux liens puis j'ai juste changé la couleur lors du passage du curseur. 

- **Problème 2 :** Le contenu reste scotché du côté gauche de l'écran quand la taille de l'écran excède la taille maximale ($1400px$) fixée.
- **Solution 2 :** Utiliser flexbox sur html.


## **II. Version tablette**
- **Problème 1 :** Les images des cartes d'hébergements les plus populaires rétrécissaient drastiquement après changement du sens d'affichage.

- **Solution 1 :** défaire la hauteur minimale spécifiée dans la version desktop. 

## **III. Version mobile**
- **Problème 1 :** Une fois le texte du bouton de recherche caché et la loupe révélée, le bouton gardait la même largeur malgré que j'avais spécifié une largeur plus petite.
- **Solution 1 :** Appliquer le style **display: contents** au bouton. 

- **Problème 2 :** La barre de recherche gardait une largeur fixe alors que la zone de recherche étais sencée s'agrandir pour que la barre occupe toute la largeur de l'écran. 
- **Solution 2 :** Lui appliquer la règle **flex-grow: 1**. 

- **Problème 3 :** La hauteur des filtres de recherche s'était réduite à celle du texte à l'interieur. 
- **Solution 3 :** Défaire la hauteur ($50px$) appliquée à toute la section filtre (**height: fit-content**) puis 
attribuer cette même hauteur aux deux divs de filtres.

- **Problème 4:** L'icone **info** tel que présent sur le site fais partie des icônes du type **régular** qui n'existe que dans la version payante de *font-awesome*.
- **Solution 4 :** Puisque je n'ai pas la version payante, j'ai juste appliqué une bordure grise de rayon $50\%$.

## **IV. Problèmes généraux***

- **Problème 1 :** Certaines images étaient rognées identiquement aux maquettes, d'autres non.
- **Solution 1 :** Toutes les images n'ont pas la vleur de la proprité **object-fit**. Les unes ont pour valeur **cover** tandis que pour d'autres ce doit être **fill**.  

