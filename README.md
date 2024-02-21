# python-course

## Les bases
En python on utilise des 'indentations'. C'est les espaces ou les tabs en début de ligne. Les indentations sont super importantes ! 
https://www.docstring.fr/glossaire/indentation/ 



### Type de données 
Les types permettent de définir le truc que l'on manipule. 
| Type de Donné   |      Type python      |  Description | Exemple d'utilisation
|-----------------|-----------------------|-----------------------------------------------------------------|--------------------------------------------------------------------------------:|
| Texte           | str                   |  Permet de stocker du texte.                                    | `nom="théo"` `adenine='A'`                                                      | 
| Nombre          | int, float, complex   |  Permet de stocker des nombres.                                 |  `age=45` `prix=2.99` `c = 3 + 4j`                                              | 
| Listes          | list                  |  Permet de stocker plusieurs éléments.                          |  `x=[0,1,2,3,4,5]` `ma_liste=["text", 1, 2.36, [1,2] ]`                         | 
| Dictionnaires   | dict                  |  Permet de stocker une correspondance entre plusieurs éléments  | ```adn={ "A" : "Adénine", "T" : "Thymine", "G": "Guanine", "C": "Cytosine" }``` | 

Pour connaitre le type de quelque chose on peut utiliser `type(x)` : 
```python
truc=2.3
print(type(truc))
```
Python va nous indiquer `<class 'float'>` car truc est un nombre flottant.

### Les boucles
Dans beaucoup de cas on vas avoir besoin de faire plusieurs foi une opération. Par exemple pour faire de l'échantillonnage, ou des sommes.
Boucler de x à y -1 en sautant de n 
```python
for i in range(1,10,2): #(initiale,finale mais non inclu, saut)
  print(i); 
  #affiche: 1,3,5,7,9
```
Boucler de x à y - 1 : 
```python
for i in range (1,4): # (initial, finale mais non inclu)
  print(i);
  #affiche: 1,2,3 note: 4 not non inclu
```
Boucler de 0 à x - 1 : 
```python
for i in range (5):
  print (i);
  #affiche: 0,1,2,3,4 note: 5 non inclu
```
Boucler sur une chaine de caractère : 
```python
sequence = "AAGGTGAGTGAAATCTCAACACGAGTATGGTTCTGAGAGTAGCTCTGTAACTCTGAGG";  
for element in sequence:
  print(element);
  #affiche:  "A" "A" "G" "G"
```

![image](https://github.com/thegostisdead/python-course/assets/25646890/f4e3d70d-49ee-49db-bcbb-06a5cba2386b)
![image](https://github.com/thegostisdead/python-course/assets/25646890/7279dc39-7cc3-4466-b1a5-13b571d63439)


### Les conditions 
Dans beaucoup de cas on a besoins de faire des tests pour faire une choses ou une autre. 
```python
if condition :
    print("faire x")
else : 
    print("faire y")
```
Exemple : tester si un nombre des supérieur à 2 :
```python
x = 45
if x > 2 :
  # faire quelque chose 
else :
  # faire autre chose
```

Si on veut faire des test sur plus de cas on peut utiliser `elif`. 
```python
if vitesse < 30:
    print('Vous roulez à 30 km/h')
elif 30 < vitesse < 50 :
    print('Votre vitesse est bonne')
elif 50 > vitesse > 130 :
    print('La vitesse est dangeureuse')
else:
    print('Plus de permis')
```

### Les fonctions
Les fonctions permettent de ré utiliser du code. Cela permet de réduire sa quantité de code. 
Une fonction porte généralement un nom qui sert à l'appeler, et possède des paramètres. Les paramètre sont des éléments variables. 
Tout le code qui est indenté sous le mot clé `def` fait parti de la fonction. 

```python
def ma_super_fonction(param1, param2):
  print(param1)
  print(param2)
```

Une fonction peut renvoyer une valeur. L'instruction `return` permet de dire : "Renvoyer la valeur ..."
Exemple : 

```python
def adition(param1, param2):
  resultat = param1 + param2
  return resultat

# appel de la fonction
toto=adition(1, 8)
print(toto)
```
9





## Pour faire des maths


## Faire des graphiques



