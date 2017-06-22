EXO 1
* je dois décallé les lettres de l'alphabet de 1 de une lettre
* trouvé la correspondance de la lettre puis la décallé de 1
* recupéré le message puis séparé de toute lettre exemple: "abc" en : 'a', 'b' etc

DEBUT

phrase <- message de l'utilisateur
alphabet <- ['a', 'b', 'c'] jusqu'a 25
    
    POUR 
        i <- 0 taille (phrase) PAS 1
        
        POUR j <- 0 taille (alphabet)
        
            SI phrase[i] = alphabet[j]
                ALORS position j     

                crypte <- crypte + alphabet[position + 1] 

            FINSI

        FINPOUR

    FINPOUR

    afficher(crypte)

FIN
---------------------------------------------------
EXO2
*comme exercice 1 mais avec un nombre de décalage
*on demande a l'utilisateur son nombre de décalage
DEBUT

phrase <- message de l'utilisateur
alphabet <- ['a', 'b', 'c'] jusqu'a 25
nbD <- nombre de décalage 

    POUR 
        i <- 0 taille (phrase) PAS 1
        
        POUR j <- 0 taille (alphabet)
        
            SI phrase[i] = alphabet[j]
                ALORS position j     

                crypte <- crypte + alphabet[position + nbD] 

            FINSI

        FINPOUR

    FINPOUR

    afficher(crypte)

FIN

---------------------------------------------------
EXO3
* comme exercice 1 mais avec une clé
* on demande à l'utilisateur son message
* on demande à l'utilisateur d'entré sa clé de cryptage

DEBUT

phrase <- message de l'utilisateur
alphabet <- creation de la clé par l'utilisateur

    POUR 
        i <- 0 taille (phrase) PAS 1
        
        POUR j <- 0 taille (alphabet)
        
            SI phrase[i] = alphabet[j]
                ALORS position j     

                crypte <- crypte + alphabet[position]

            FINSI

        FINPOUR

    FINPOUR

    afficher(crypte)

FIN