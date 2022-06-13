voyons voir si tout fonctionne
mais ca marche

# Define Sequential model with 3 layers
model = keras.Sequential(
    [
        layers.Dense(2, activation="relu", name="layer1"),
        layers.Dense(3, activation="relu", name="layer2"),
        layers.Dense(4, name="layer3"),
    ]
)
# Call model on a test input
x = tf.ones((3, 3))
y = model(x)





    git status : permet de visualiser quel est l'état du repository.
    git add fichiers repertoires : permet d'indiquer que ces fichiers/répertoires doivent être ajouter au repository.
    git commit -m "Un commentaire" : permet de valider le ou les git add effectué avant.
    git push : permet d'envoyer vos commits en attentes sur GitHub (demande votre login dans la console puis votre mot de passe dans une fenêtre, voir captures).


Création d'un modèle séquentiel

Vous pouvez créer un modèle séquentiel en transmettant une liste de couches au modèle séquentiel constructeur: 

model = keras.Sequential(
    [
        layers.Dense(2, activation="relu"),
        layers.Dense(3, activation="relu"),
        layers.Dense(4),
    ]
)
