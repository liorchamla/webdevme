# Conception et exploitation d'une base de données SQL

L'apprentissage de base du langage SQL ne suffit pas à concevoir et à exploiter correctement une base de données relationnelle, il faut pour cela une grande réflexion en amont.

# Formation(s) vidéo

Comme chaque mois, une ou plusieurs formations vidéo viennent appuyer notre apprentissage !

## Les bases du SQL (LDD et LMD)

_Formation disponible sur l'espace communautaire_

## La méthode MERISE : Du Dictionnaire des Données au Modèle Physique des Données

_Formation disponible sur l'espace communautaire_

# Projet du mois

Une entreprise d'import / export de jouets vous demande de revoir de fond en comble leur système d'informations afin de se doter à termes d'un ERP qui leur permettra de gérer la majorité des aspects de son activité via un logiciel unique et centralisé. Evidemment, l'entreprise elle même se divise en plusieurs services dont chacun gère un aspect : Ressources humaines, achats, ventes, SAV etc.

Vous trouverez ci dessous une description de certains de ces services afin de vous aiguiller dans la conception du futur SI.

## Service Achats

Ce service est dédié au "sourcing", son activité principale est de trouver des produits intéressants à l'étranger, de discuter avec les potentiels fournisseurs puis d'acheter et acheminer les produits vers la France.

### Sourcing de produits et de fournisseurs potentiels

Lorsque le service achat découvre un produit intéressant, il répertorie les informations intéressantes (nom du produit, description, poids en grammes, public visé ...) ainsi que les fournisseurs qui sont capables de fournir ce produit (attention, les fournisseurs n'ont pas forcément le même prix de vente pour le même produit).

**Les produits qui sont trouvés par le service achat forment le catalogue de l'entreprise.**

### Commandes fournisseurs / Factures fournisseurs / Réglements fournisseurs

Enfin, le service achat a la responsabilité de commander des produits auprès des fournisseurs : une commande est passée auprès d'un seul fournisseur et peut concerner un ou plusieurs produits. Dans l'idéal, l'entreprise aimerait conserver la trace de la personne qui a passé la commande.

Lorsque le fournisseur reçoit la commande, il envoie au service achats la facture correspondante. Lors du paiement, c'est au service achats de conserver la trace du ou des paiements qui seront rattachés à la facture.

## Service Ventes

Ce service a pour mission de trouver des clients et de vendre les produits référencés dans le catalogue.

### Clients

La mission première des équipes du service Ventes est de trouver et de référencer des clients intéressés par l'activité de l'entreprise afin, à termes, de réaliser des ventes.

### Devis / Factures clients / Réglements clients

Lorsqu'un client est intéressé par un ou plusieurs produits, le service des ventes lui fait parvenir un devis correspondant qui peut ensuite être accepté ou refusé par le client. Si le client accepte le devis, le service lui fait alors parvenir une facture et gardera ensuite la trace du ou des paiements que le client va exécuter afin de régler cette facture.

On gardera évidemment la trace de l'employé qui a fait le devis afin de mettre en place des politiques d'objectifs et de récompenses.

## Service RH

Le service RH a pour mission de gérer les salariés des différents services de l'entreprise. Dans l'entreprise, le fonctionnement est le même pour tous les services : chacun d'entre eux est dirrigé par une personne précise (notons que la même personne peut diriger plusieurs services, c'est une situation qui est arrivée dans l'histoire de l'entreprise) qui a donc _sous ses ordres_ le reste des employés du service.

Evidemment, le service RH tient l'historique des rémunérations de chaque salarié. Attention, on ne parle pas ici des fiches de paie (qui sont gérées par le service comptable et qui n'a pas d'intérêt dans ce projet). Ce qui intéresse le service RH, c'est de savoir quelle est la rémunération actuelle d'un salarié et quelles étaient ses anciennes rémunérations. Ainsi, on peut voir l'évolution de la rémunération pour chaque salarié et à quels moments celle ci a évolué.

# Débutants : On numérise le service RH

Votre mission sera de réfléchir, concevoir et réaliser la structure de données qui sera capable de stocker **les données du service RH**.

Pour cela vous utiliserez certains outils de la méthode MERISE :

- Le dictionnaire des données ;
- Le modèle conceptuel des données (dit "entités associations") ;
- Le modèle physique des données ;

Une fois que la structure vous semble bonne, vous devrez créer la base de données et la remplir avec des données d'exemple afin de vous assurer que vous êtes capables d'effectuer les requêtes suivantes :

- Récupérer la liste des employés d'un service donné en ordonnant par rémunération actuelle décroissante
- Récupérer les évolutions de rémunération d'un salarié donné en ordonnant par année de façon décroissante (un historique des évolutions)
- Récupérer le nombre total d'employés de chaque service ainsi que la rémunération totale de ses employés (ce que coûte chaque service à l'entreprise)

# Avancés : On numérise tout le SI

Votre mission sera de réfléchir, concevoir et réaliser la structure de données qui sera capable de stocker **toutes les données du SI**.

Pour cela vous utiliserez certains outils de la méthode MERISE :

- Le dictionnaire des données ;
- Le modèle conceptuel des données (dit "entités associations") ;
- Le modèle physique des données ;

Une fois que la structure vous semble bonne, vous devrez créer la base de données et la remplir avec des données d'exemple afin de vous assurer que vous êtes capables d'effectuer les requêtes suivantes :

- Récupérer le catalogue des produits
- Récupérer la liste des commandes clients ordonnées par date de commande descendante (de la plus récente à la plus ancienne)
- Récupérer la liste des factures clients ordonnées par date de commande descendante (de la plus récente à la plus ancienne)
- Récupérer le nombre total de commandes clients par employés qui ont effectué ces commandes
- Récupérer la liste des réglements clients ordonnés par date du réglement

# Journée WebDevMe

Comme tous les mois, une journée où on se retrouve tous pour revoir les notions abordées, en discuter, pratiquer et enseigner les uns aux autres.

## Workshop du matin

- Revue des réalisations des étudiants volontaires qui veulent présenter aux autres leur réfléxion et leurs résultats
- Discussions et questions / réponses

## Séminaire mensuel

A vous de nous apprendre des choses ! Profitez de l'occasion qui vous est donné pour proposer un sujet de conférence que vous donnerez vous mêmes. Les sujets ne manquent pas :

- Indexation
- Performances
- Fonctionnalités "cachées" / peu connues du SQL
- SGBDs différents / Bases de données NoSQL
