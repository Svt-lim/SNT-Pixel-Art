# Activité SNT seconde : Générateur de pixel-art.
# Pré-requis :
Ouvrez le trinket de base du projet : [jumpto.cc/web-pixel](https://trinket.io/embed/html/705f264f59#.XftFuVPfswB)
vous avez trois onglets : Index.html, Style CSS et script.js
![Depart](https://github.com/Svt-lim/SNT/blob/master/images/1%20pixel-starter.png)
# Etape 1: Faire la matrice
Dans l'onglet Index.html entre ```<body>``` et ```</body>``` vous allez créer un ```<div>```
![Depart](https://github.com/Svt-lim/SNT/blob/master/images/2%20pixel-art-art.png)  
un ```<div>``` est objet invisible auquel vous allez donner un style. 
* ouvrez l'onglet CSS et creer un style pour votre ```<div>```  
![image](https://github.com/Svt-lim/SNT/blob/master/images/3%20pixel-art-style.png)  
Félicitations vous avez créer un pixel noir !  
il va falloir peupler votre fichier Index.html de pixel organisés en rangées et colonnes  
* retournez dans votre fichier index.html et inserez 3 pixels  
![image](https://github.com/Svt-lim/SNT/blob/master/images/4%20pixel-art-row.png)  
Notez que vous utilisez une ```class``` plutôt qu'un ```id```. une ```class``` est plus utile car vous allez devoir creer 64 pixels.  
* retournez dans style.CSS afin de creer un style pour les class pixel & row  
![image](https://github.com/Svt-lim/SNT/blob/master/images/5%20pixel-art-row-style.png)  
* dans votre fichier index.html, ajouter deux sections de 3 pixels pour obtenir une matrice de 3x3  
![image](https://github.com/Svt-lim/SNT/blob/master/images/6%20pixel-art-grid-3.png)  
***
# Défi 1 : Amenez votre matrice à 8x8 cases.
***  
# Etape 2 : Interagir avec les pixels  
A l'aide d'un peu de Javascript vous allez colorer un pixel en cliquant dessus. Vous allez créer une fonction et l'appeller pour noircir vos pixels.  
* dans l'onglet script.js ajoutez le code suivant :  
![image](https://github.com/Svt-lim/SNT/blob/master/images/8%20pixel-art-set-pixel-colour.png)  
pour l'instant votre fonction ne produit aucun effet car il faut l'appeler dans Index.html.  
* retournez dans Index.html et modifiez le ```<div>``` de votre premier pixel.  
![image](https://github.com/Svt-lim/SNT/blob/master/images/9%20pixel-art-onclick.png)  
le **this** ici est juste un moyen de se rappeller que la fonction n'est appelée que pour **ce** pixel.  
* testez votre code en cliquant sur votre premier pixel vous devriez obtenir ça :  
![image](https://github.com/Svt-lim/SNT/blob/master/images/10%20pixel-art-black.png)  
***
# Défi 2 : Rendez chaque pixel cliquable et coloriable en noir.
***
**astuce : vous pouvez cliquer sur Autorun pour effacer vos pixels**  
# Etape 3 : Creer une palette de couleur.  
* ajoutez le code suivant dans votre fichier CSS pour creer un style de pinceau 
![image](https://github.com/Svt-lim/SNT/blob/master/images/12%20pixel-art-pen.png)  
* retournez dans votre fichier index.html et incluez le code suivant entre body et votre div "art"  
![image](https://github.com/Svt-lim/SNT/blob/master/images/13%20pixel-art-palette.png)  
la balise style= permet d'ajouter directement du CSS dans le fichier HTML ce qui ici nous évite de trop jongler entre les fichiers.  
* ouvrez votre script.js et ajoutez le code suivant tout en haut du script, en ligne 1 :  
![image](https://github.com/Svt-lim/SNT/blob/master/images/15%20pixel-art-set-pen.png)  
* il faut aussi changer la fonction **setPixelColour** pour utiliser **Pencolor** au lieu de **black**  
![image](https://github.com/Svt-lim/SNT/blob/master/images/pixel-art-use-pen.png)  
* modifiez votre palette dans votre fichier index.html  
![image](https://github.com/Svt-lim/SNT/blob/master/images/16%20pixel-art-palette-onclick.png)  
# Défi 3 : Ajoutez les couleurs Rouge, Vert et Bleu à votre palette  
***
![image](https://github.com/Svt-lim/SNT/blob/master/images/pixel-art-final.png)



