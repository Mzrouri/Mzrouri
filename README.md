def calcul_quantite_stock(longueur_boite, largeur_boite, hauteur_boite, longueur_emb, largeur_emb, hauteur_emb):
    # Calculer le nombre de boîtes dans une seule couche
    nb_boites_couche_longueur = longueur_emb // longueur_boite
    nb_boites_couche_largeur = largeur_emb // largeur_boite
    nb_boites_couche_hauteur = hauteur_emb // hauteur_boite
    nb_boites_couche = nb_boites_couche_longueur * nb_boites_couche_largeur * nb_boites_couche_hauteur

    # Calculer le nombre total de boîtes pouvant être stockées
    nb_total_boites = nb_boites_couche

    # Calculer le nombre de couches possibles
    nb_couches = hauteur_emb // hauteur_boite

    # Afficher les résultats
    print(f"Quantité stock dans l'emballage : {nb_total_boites}")
    print(f"Nombre de boîtes par couche : {nb_boites_couche}")
    print(f"Nombre de couches : {nb_couches}")

# Exemple d'utilisation
calcul_quantite_stock(20, 10, 5, 100, 50, 30)

