# tp-js

# Fait grace a chat gpt ( je ne savais pas quoi mettre dans un readme)

Ce code est une page HTML qui permet d'interagir avec l'API de Pokémons pour afficher des informations sur ces derniers et pour effectuer des calculs avec des noms et prénoms donnés.
### Structure HTML

Le fichier HTML contient plusieurs éléments :
- Des liens vers des feuilles de style (style.css et bootstrap.min.css)
- Un bouton qui, lorsqu'il est cliqué, affiche les noms des 3 starters originaux de Pokémon ainsi que leurs évolutions
- Un formulaire permettant d'entrer un nom et un prénom pour calculer un chiffre entre 1 et 1008 qui correspond à un Pokémon en particulier
- Un menu déroulant permettant de sélectionner un nombre entre 1 et 1008
- Un bouton pour valider la sélection dans le menu déroulant
- Un élément de paragraphe pour afficher le nom du Pokémon sélectionné
- Un élément de conteneur d'image pour afficher l'image du Pokémon sélectionné
### Structure JavaScript

Le fichier JavaScript contient plusieurs fonctions : 
- `sumOfLettersPositions(word)`: cette fonction prend un mot en entrée et calcule la somme des positions de chaque lettre de l'alphabet dans ce mot (en commençant à 1 pour la lettre a). Elle renvoie un nombre entier. 
- `calculerChiffre()`: cette fonction récupère les valeurs des champs nom et prénom du formulaire, calcule un nombre en utilisant la fonction `sumOfLettersPositions()`, et affecte ce nombre au champ chiffre. Elle renvoie également ce nombre. 
- `fetchSomePokemons()`: cette fonction utilise l'API de Pokémons pour récupérer une liste de tous les Pokémon disponibles. Elle renvoie une promesse qui sera résolue avec la liste. 
- `myButton.addEventListener()`: cette fonction est appelée lorsqu'on clique sur le bouton "Afficher les 3 starters originaux". Elle utilise la fonction `fetchSomePokemons()` pour récupérer la liste de tous les Pokémon et affiche les noms des 3 starters originaux ainsi que leurs évolutions dans un élément de paragraphe. 
- `selectButton.addEventListener()`: cette fonction est appelée lorsqu'on clique sur le bouton "Valider" dans le menu déroulant. Elle utilise l'API de Pokémons pour récupérer les informations sur le Pokémon correspondant au nombre sélectionné dans le menu déroulant. Elle affiche le nom de ce Pokémon dans un élément de paragraphe et affiche également son image dans un élément de conteneur d'image.
### Utilisation

Pour utiliser cette page, il suffit de l'ouvrir dans un navigateur web et de cliquer sur les différents boutons ou de remplir le formulaire. Les noms des Pokémon ainsi que leurs images seront affichés en fonction des actions effectuées. Notez que cette page nécessite une connexion internet pour fonctionner, car elle utilise l'API de Pokémons.
