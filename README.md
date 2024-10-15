Début
    // Initialiser les compteurs
    longueur = 0
    nombre_mots = 0
    nombre_voyelles = 0
    
    // Liste des voyelles
    voyelles = "aeiouyAEIOUY"

    // Lire la phrase caractère par caractère
    Lire caractère
    Tant que caractère != '.'
        longueur = longueur + 1

        // Vérifier si le caractère est une voyelle
        Si caractère est dans voyelles alors
            nombre_voyelles = nombre_voyelles + 1
        Fin Si
        
        // Vérifier si le caractère est un espace
        Si caractère == ' ' alors
            nombre_mots = nombre_mots + 1
        Fin Si

        // Lire le prochain caractère
        Lire caractère
    Fin Tant que

    // Ajouter 1 au nombre de mots pour le dernier mot
    Si longueur > 0 alors
        nombre_mots = nombre_mots + 1
    Fin Si

    // Afficher les résultats
    Afficher "Longueur de la phrase : ", longueur
    Afficher "Nombre de mots : ", nombre_mots
    Afficher "Nombre de voyelles : ", nombre_voyelles
Fin
