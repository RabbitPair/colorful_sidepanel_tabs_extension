# Journal des modifications

Tous les changements notables apportés à ce projet seront documentés dans ce fichier.

Ce projet adhère à la [Gestion Sémantique des Versions](https://semver.org/).

----
## [2.10.0] - 2024-10-01

### Ajouté
- **Document Picture-in-Picture** : Introduction de l'Image dans l'Image Avancée, disponible en essai gratuit avant la sortie officielle de la version premium de l'extension. Lorsqu'elle est activée, elle prend le pas sur l'Image dans l'Image standard. Si la page actuelle ne la prend pas en charge, le mode standard sera utilisé. L'Image dans l'Image Avancée dispose d'un lecteur vidéo personnalisé avec des fonctionnalités telles que :
  * **Lire/Pause vidéo** (Espace ou K)
  * **Ajuster le volume** (Flèche Haut/Bas)
  * **Muet/Démuet vidéo** (M)
  * **Avance rapide/Retour rapide vidéo** (Flèche Gauche/Droite ou Molette de la souris)
  * **Avance rapide/Retour rapide vidéo de 5 secondes** (Flèche Gauche/Droite)
  * **Avance rapide/Retour rapide vidéo de 10 secondes** (J/L)
  * **Lire la vidéo suivante** (Shift + N)
  * **Lire la vidéo précédente** (Shift + P)
  * **Afficher les sous-titres** (pris en charge sur certains sites comme youtube.com, vimeo.com, tver.jp, etc.) (C)
  * **Afficher les commentaires** (pris en charge sur certains sites comme nicovideo.jp, bilibili.com, etc.) (D)
  * **Quitter l'Image dans l'Image** (Esc)
  * **Basculer entre masquer/afficher la vidéo et lire/pause** (Q)
  * **Basculer en plein écran** (F)
  * **Ajuster la vitesse de lecture** ( > ou <)
  * **Aller au début/à la fin de la vidéo** (Home/End)
  * **Aller à un pourcentage de la vidéo** (0-9)
  * **Ajuster la fenêtre à la taille de la vidéo** (W)
  * **Basculer l'Image dans l'Image depuis la page principale** (Alt + P)
  
  > Si les sites que vous visitez fréquemment prennent en charge les sous-titres ou les commentaires, vous pouvez soumettre un [problème : Image dans l'Image Avancée](https://github.com/RabbitPair/colorful_sidepanel_tabs_extension/issues/new?assignees=&labels=&projects=&template=Advanced-Picture-in-Picture.md&title=), et nous l'adapterons dès que possible. Veuillez noter que certains sites peuvent avoir des restrictions régionales, nécessitant des informations supplémentaires.
- **Raccourci pour l'Image dans l'Image** : Un nouveau raccourci clavier Alt+P a été ajouté pour basculer rapidement en mode Image dans l'Image. Cela permet aux utilisateurs de passer facilement les vidéos en vue Image dans l'Image sans utiliser la souris, améliorant ainsi la productivité et les capacités multitâches.
- **Basculer l'Image dans l'Image dans la barre de navigation inférieure** : Vous pouvez maintenant ajouter une option de basculement de l'Image dans l'Image à la barre de navigation inférieure. Cela peut être configuré dans les paramètres d'apparence sous "Afficher la barre de navigation inférieure" - "Configurer".
- **Trier les onglets par URL** : Une nouvelle option de menu "Trier les onglets par URL" a été ajoutée au menu "Plus".
- **Comportement de réduction du groupe d'onglets** : Une nouvelle option "Comportement de réduction du groupe d'onglets" a été ajoutée au menu "Groupe d'onglets avancé". Vous pouvez modifier le comportement de réduction des groupes d'onglets dans le navigateur. Les options incluent : 'Afficher le groupe actuel et réduire les autres groupes', 'Développer tous les groupes' et 'Utiliser les paramètres par défaut du navigateur'.
- **Paramètres du site** : Trois nouvelles options ont été ajoutées aux paramètres du site :
  * **Action de restriction de l'Image dans l'Image** : Configurer l'action pour les restrictions de l'Image dans l'Image.
  * **Entrer automatiquement en mode Image dans l'Image** : Entrer automatiquement en mode Image dans l'Image lorsqu'une vidéo est présente lors de l'entrée sur la page.
  * **Paramètres des sous-titres** : Configurer les sélecteurs CSS pour l'élément de sous-titres et son parent sur la page.

### Modifié
- Lorsque l'onglet du panneau latéral n'est pas ouvert, si "Image dans l'Image lors du changement d'onglet" est activé (activé par défaut), il passera automatiquement en mode Image dans l'Image (Rappel important : une interaction utilisateur est requise, comme cliquer sur la page lisant la vidéo pour activer l'interaction utilisateur).
- Lors de la fermeture de la barre latérale de la page, elle est maintenant supprimée au lieu d'être masquée. Elle réapparaîtra uniquement après actualisation de la page.

### Corrigé
- Correction du problème où la liste d'accès rapide ne gérait pas plusieurs URL.

----

## [2.9.0] - 2024-09-15

- Ajout de **Effacer les onglets** : Enregistrez un instantané et fermez tous les onglets sauf celui actif. Restaurez-les à partir des onglets récemment fermés ou des instantanés.
- Ajout de **Activation automatique du regroupement des onglets** : Créez automatiquement un nouveau groupe lors de l'ouverture d'un nouvel onglet. Les onglets suivants ouverts à partir de cet onglet rejoindront le groupe.
- Ajout de **Espacement vertical de la liste** : Nouvelle option dans les paramètres de groupe d'onglets avancés pour ajuster l'espacement vertical des éléments de la liste.
- Ajout de **Ajouter plusieurs URL à l'accès rapide** : Permet d'ajouter des groupes et de sélectionner plusieurs onglets à enregistrer dans l'accès rapide.
- Ajout de **Espacement des éléments d'accès rapide** : Définissez l'espacement vertical/horizontal des éléments d'accès rapide dans la page des options.

---
## [2.8.0] - 2024-09-12

### Ajouté
- Ajout de **Historique des onglets** : Vous pouvez maintenant facilement voir quels sites Web ont été ouverts sous le même onglet. Cliquez avec le bouton gauche pour ouvrir le site Web dans l'onglet actuel, cliquez avec le bouton du milieu ou Ctrl+clic gauche pour ouvrir le site Web dans un nouvel onglet. Pour plus de détails, veuillez consulter la page des options.
- Ajout de **Noms de groupe personnalisés** : Dans la page des options - Groupe d'onglets avancé, vous pouvez ajouter ici quelques groupes prédéfinis, afin de pouvoir les sélectionner rapidement lorsque vous devez ajouter des onglets à un groupe. Nous avons déjà prédéfini certains noms de groupe, que vous pouvez modifier ou supprimer selon vos besoins.
- Ajout de **Utiliser le nom du dossier de signet comme nom de groupe** : Dans la page des options - Groupe d'onglets avancé, une nouvelle option a été ajoutée. Si le site Web ouvert est un signet, il sera automatiquement ajouté au groupe, et le nom du groupe utilisera le nom du répertoire de signets.
- Ajout de **Index d'onglet** : Dans la page des options, lorsque activé, l'index de l'onglet sera affiché à côté du titre, facilitant l'activation de l'onglet en utilisant [Ctrl+nombre] sur Windows ou [cmd+nombre] sur Mac. Exemple : 1. stackoverflow.com 2. youtube, de sorte qu'il est facile de faire Ctrl + 2 sur Windows ou cmd + 2 sur Mac pour aller sur youtube
- **Paramètres du site optimisés** : Amélioration de l'option pour définir la couleur de fond et la couleur de la police pour les sites.

### Modifié
- Lors de la vérification des signets, permettre la mise à jour des URL redirigés. Si l'URL n'est pas accessible, afficher les codes d'erreur : Réponses réussies (200 – 299), Messages de redirection (300 – 399), Réponses d'erreur client (400 – 499), Réponses d'erreur serveur (500 – 599). Pour plus de détails, veuillez consulter : https://developer.mozilla.org/en-US/docs/Web/HTTP/Status

### Corrigé
- Correction du problème où la fenêtre contextuelle de modification du signet ne disparaissait pas

## [2.7.0] - 2024-09-05
### Ajouté
- Ajout de la **gestion des favoris** : Ajout de la fonctionnalité complète de gestion des favoris
- Ajout de la **barre de navigation des onglets** : options d'apparence, affichage : onglets, favoris, historique, onglets récemment fermés, liste de lecture et accès rapide dans le panneau latéral
- Ajout du menu **Ajouter un onglet au groupe** : ajouter des onglets à un nouveau groupe ou à un groupe existant
- Ajout de la mise en évidence des mots-clés de recherche
- Ajout de la réservation de l'édition Premium
### Modifié
- Ajustement des autorisations de Cookie, ReadingList et favoris en autorisations optionnelles, nécessitant l'autorisation de l'utilisateur pour être utilisées
### Obsolète
- **Page des options - Historique - Afficher dans le panneau latéral** : Cette option a été remplacée par la *barre de navigation des onglets* et sera bientôt obsolète

### Corrigé
- Correction du problème où le bouton d'extension de groupe n'apparaissait pas lors du premier clic sur la barre latérale
- Correction du problème où la réouverture du navigateur et le clic sur l'icône de l'extension nécessitaient de resélectionner entre popup ou barre latérale
- Correction du problème où les tailles des icônes des onglets épinglés et des icônes d'accès rapide étaient incohérentes

---

## [2.6.1] - 2024-08-30

### Modifié
- Méthode d'affichage du menu optimisée, amélioration des messages d'erreur
- Ajout de plus de compatibilité pour les navigateurs basés sur Chromium


---

## [2.6.0] - 2024-08-28
### Ajouté
- Ajout de **Zoom du menu des onglets** : Une fonctionnalité de zoom a été ajoutée au menu des onglets, vous permettant d'ajuster librement le niveau de zoom de 1% à 1000%.

### Modifié
- L'accès rapide a été déplacé vers un élément de menu séparé.
- Tri par glisser-déposer optimisé

### Corrigé
- Correction d'un problème où certaines zones ne changeaient pas après avoir modifié la couleur de la police.

### Obsolète
- **Accès rapide dans le menu des onglets** : L'accès rapide a été déplacé vers un élément de menu séparé. L'option dans le menu des onglets sera bientôt obsolète (la fonctionnalité reste la même).

### Supprimé
- Suppression de l'option de zoom dans les paramètres du site car l'ajustement du zoom dans le menu ne fournissait pas un aperçu intuitif des modifications. La fonctionnalité de zoom a été déplacée vers le menu des onglets pour un aperçu en temps réel.

---

## [2.5.2] - 2024-08-27

### Corrigé

- Correction du problème où les images de fond enregistrées étaient perdues après le redémarrage de l'application
- Correction du problème où la fermeture de tous les onglets du même site dans toutes les fenêtres échouait
- Correction du crash lors de la désactivation de DnD

------

## [2.5.0] - 2024-08-25

### Ajouté

- Prise en charge du tri par glisser-déposer des onglets et des groupes dans l'ordre des onglets, et synchronisation avec Chrome
- Synchronisation de l'état d'expansion du groupe avec Chrome

### Corrigé
- Correction du problème où le téléchargement d'un fichier d'image de fond trop volumineux provoquait une erreur de dépassement de quota QUOTA_BYTES
- Correction du problème où l'affichage de tous les onglets de la fenêtre provoquait une erreur et le regroupement par site échouait


---

## [2.4.0] - 2024-08-20

### Ajouté
- ajout de **Télécharger une image de fond** : Vous pouvez télécharger une image depuis votre appareil local pour l'utiliser comme fond.
- ajout de **Couleur de fond personnalisée** : Prend désormais en charge les couleurs de fond personnalisées, et vous pouvez également choisir une couleur pour générer un beau dégradé

### Modifié

- **couleur de la police** : La couleur de la police changera automatiquement en noir ou blanc en fonction de la couleur dominante du fond ou de l'image de fond. Si l'image est grande, il peut falloir un certain temps pour appliquer le fond, ce qui est normal.

### Corrigé
- Correction du problème où certaines zones ne changeaient pas après avoir modifié la couleur de la police

### Obsolète
- **Style de fond de liste** : Cette fonctionnalité définit le style de fond pour chaque liste, avec quelques couleurs de dégradé intégrées. Cependant, avec la sortie des couleurs de fond personnalisées, sa mission est terminée et elle sera bientôt supprimée.

---

## [2.3.0] - 2024-08-16

### Ajouté
- ajout de **Barre latérale sur les pages** : La barre latérale de la page vous permet d'injecter une barre latérale dans les pages web que vous consultez sans ouvrir la barre latérale du navigateur pour gérer les onglets. C'est une fonctionnalité très utile pour les utilisateurs avec des résolutions d'écran plus petites qui trouvent la barre latérale du navigateur trop large et non ajustable. Cependant, en raison de certaines restrictions, la barre latérale de la page n'offre que des fonctionnalités très limitées. Lorsque cette fonctionnalité est activée, vous pouvez utiliser la souris pour survoler le bord de la fenêtre pour faire apparaître la barre latérale.

### Supprimé
- suppression de **Boule flottante**

---

## [2.2.0] - 2024-08-14

### Ajouté
- Nouveau menu d'onglets **Garder l'onglet actif** : Gardez l'onglet actif pour qu'il ne soit pas automatiquement supprimé.

### Modifié
- Performances optimisées et taille du bundle réduite.

---

## [2.1.0] - 2024-08-10

### Ajouté
- Enregistrer automatiquement les instantanés de fenêtre, de groupe et d'onglet. Après le redémarrage du navigateur, si une seule fenêtre est ouverte et que moins de 5 nouveaux onglets sont ouverts, un toast vous invitera à restaurer la dernière fenêtre et les informations d'onglet enregistrées lorsque la barre latérale est ouverte.

### Modifié
- Optimisation des données de stockage pour un accès rapide afin d'accélérer le temps d'accès.

### Corrigé
- Correction d'autres problèmes mineurs.

---

## [2.0.1] - 2024-08-09

### Corrigé
- Correction du format du message pour l'importation réussie d'instantanés.
- Correction du problème où les importations en double provoquaient des entrées d'accès rapide répétées.

---

## [2.0.0] - 2024-08-08

### Modifié
- Renommé l'extension de "Onglets de panneau latéral coloré" à **"VertiTab - Onglets verticaux du panneau latéral"**.

### Ajouté
- Instantanés : Ajout d'une fonctionnalité de sauvegarde instantanée des onglets du navigateur en un clic. Vous pouvez enregistrer des instantanés avant de fermer le navigateur et les restaurer rapidement la prochaine fois que vous l'ouvrez. Actuellement, jusqu'à 50 instantanés peuvent être enregistrés.
- Barre de navigation inférieure améliorée : Accédez à plus de fonctionnalités depuis la barre de navigation inférieure, telles que les favoris, l'historique, les onglets récemment fermés, la liste de lecture, l'accès rapide, ouvrir un nouvel onglet, créer un instantané, rechercher, réduire les groupes, etc.
- Fonctionnalité d'importation/exportation mise à jour : Amélioration des options d'importation et d'exportation pour mieux gérer les onglets sur différents appareils.

### Corrigé
- Corrections de bugs et améliorations de la stabilité.

---

## [1.3.3] - 2022-08-04

### Ajouté
- **Paramètres de lien** : Les paramètres du site incluent désormais une nouvelle option qui vous permet d'ajouter des règles pour contrôler si les liens du site s'ouvrent dans l'onglet actuel ou dans un nouvel onglet.

---

## [1.3.2] - 2024-08-02

### Corrigé
- Correction du problème où le clic sur le bouton central de la souris pour fermer l'onglet ne fonctionnait pas.

---

## [1.3.1] - 2024-08-01

### Modifié
- Optimisation de la disposition de l'accès rapide et ajout de la prise en charge du tri par glisser-déposer.
- Amélioration de la logique d'expansion de tous les groupes et de mémorisation de leur état.

### Corrigé
- Correction du problème où l'importation des données d'accès rapide échouait lorsque le panneau latéral n'était pas ouvert.
- Correction du problème où les icônes étaient mal alignées dans la vue de groupe.
- Correction d'autres problèmes mineurs.

---

## [1.3.0] - 2024-07-30

### Ajouté
- **Importation/Exportation** : Exportation des préférences utilisateur, de l'accès rapide, des paramètres du site web et des données des onglets récemment fermés, et importation dans un autre navigateur pour synchroniser les données de l'extension.
- **Sélectionner l'accès rapide depuis l'historique** : Vous pouvez rechercher les sites web les plus visités depuis l'historique et les ajouter à l'accès rapide.
- **Plus d'options dans la barre d'outils** : Ajout de plus d'options à la barre d'outils. Vous pouvez masquer l'étiquette dans la barre d'outils et contrôler les icônes affichées dans la barre d'outils.

### Modifié
- **Boîte de recherche** : La boîte de recherche prend désormais en charge la touche Entrée pour rechercher des mots-clés dans un nouvel onglet. S'il n'y a pas d'onglet ou d'historique correspondant après avoir entré le mot-clé, vous pouvez appuyer sur Entrée pour rechercher en utilisant le moteur de recherche par défaut.
- **Initialisation des données** : Ajustement du timing de l'initialisation des données et optimisation du rendu répété causé par les modifications des données.
- **URL du journal des modifications** : Mise à jour de l'URL du journal des modifications vers l'URL de publication sur GitHub.
- **Optimisation de la disposition** : Optimisation des modifications de disposition lorsque la taille de la fenêtre change.
- **Enregistrement des journaux d'erreurs** : Utilisation de Sentry pour collecter les journaux d'erreurs. Soyez assuré que cette fonctionnalité ne collectera pas vos données privées.

### Corrigé
- **Erreur de position de l'infobulle** : Correction du problème où l'infobulle clignotait lors du changement de thèmes et de vues dans la barre d'outils.
- **Navigation inférieure** : Correction du problème où la navigation inférieure bloquait la liste lorsque de nombreux onglets étaient ouverts.

---
## [1.2.3] - 2024-07-23

### Corrigé
- Correction du calcul incorrect de la hauteur de défilement de la liste lorsque les onglets épinglés et les icônes d'accès rapide dépassent 1 ligne.

### Modifié
- Modification de l'exclusion des onglets inactifs pour exclure les onglets épinglés.
- Modification de la fermeture de tous les onglets exclus pour exclure les onglets épinglés.
- Ajustement de la taille des icônes épinglées et d'accès rapide.

---

## [1.2.2] - 2024-07-19

### Ajouté
- Ajout de l'accès rapide : Vous pouvez configurer un onglet pour qu'il apparaisse dans l'accès rapide afin qu'il soit facile à trouver. Il suffit de faire un clic droit (ou un appui long) et de sélectionner Épingler à l'accès rapide. Désépingler-le lorsque vous n'en avez plus besoin en faisant un clic droit (ou un appui long) et en sélectionnant Supprimer de l'accès rapide. La différence avec les onglets épinglés est que l'accès rapide enregistre l'URL et ouvre un nouvel onglet à chaque fois qu'on clique dessus.

### Modifié
- Les onglets épinglés n'affichent que des icônes pour éviter qu'ils ne soient cliqués accidentellement et désépinglés.
- Modification de la taille des icônes des onglets épinglés.

---

## [1.2.1] - 2022-07-17

### Ajouté
- Ajout d'un nouveau menu à la navigation inférieure : exclure les onglets inactifs.
- Ajout d'un nouveau menu à la navigation inférieure : fermer tous les onglets exclus.

### Modifié
- Les modifications du menu de navigation inférieure "Grouper par site" n'affectent que la fenêtre actuelle.

### Corrigé
- Correction du problème où l'interface utilisateur sautait en raison d'une incohérence de hauteur lors du changement d'onglets actifs dans la liste.

---

## [1.2.0] - 2024-07-16

### Ajouté
- Ajout de configurations de site : Personnalisez les paramètres spécifiques au site, tels que la désactivation du mode Image dans l'image, la désactivation du mode de mise en veille automatique, et plus encore.

### Corrigé
- Correction de la création ou de la jonction automatique au même groupe de domaine : Résolution d'un problème où la création ou la jonction automatique aux mêmes groupes de domaine ne fonctionnait pas lors de la mise à jour d'un onglet.
- Correction du problème de non-réception des messages de mise à jour de configuration par la page : Assuré que les pages reçoivent correctement les messages de mise à jour de configuration.
- Correction d'autres bugs : Résolution de divers autres bugs pour améliorer la stabilité et les performances.

### Modifié
- Ajout d'une option pour afficher le bouton de fermeture au survol : Ajout d'une option pour afficher le bouton de fermeture uniquement lors du survol d'un onglet.

---

## [1.1.0] - 2024-07-13

### Ajouté
- Ajout d'options de performance : Introduction de nouveaux paramètres de performance pour personnaliser et améliorer votre expérience de navigation.
- Ajout d'une icône de défilement vers l'onglet actif : Naviguez facilement vers l'onglet actif avec une nouvelle icône de défilement vers l'onglet actif.
- Ajout de tri des onglets par domaine : Organisez vos onglets par domaine avec une nouvelle fonctionnalité de tri.
- Muet tous les onglets émettant des sons : Mettez rapidement en sourdine tous les onglets qui émettent des sons pour une expérience de navigation plus silencieuse.

### Modifié
- Suppression de l'icône de restauration : L'icône de restauration a été supprimée et remplacée par une opacité de texte de liste définie à 0,5 pour un aspect plus propre.

### Obsolète
- Suppression du tri par glisser-déposer : La solution actuelle pour le tri par glisser-déposer présente des problèmes de performance et a été temporairement supprimée.

---

## [1.0.4] - 2024-07-09

### Ajouté
- Tri par glisser-déposer pour les onglets : Réorganisez facilement vos onglets avec la fonctionnalité de glisser-déposer.

### Modifié
- Optimisation de la vitesse de chargement des pages : Amélioration supplémentaire de la vitesse de chargement des pages pour une expérience de navigation encore plus fluide.

---

## [1.0.3] - 2024-07-05

### Corrigé
- Correction de l'erreur du menu de vue mixte : Résolution d'un problème où le menu de vue mixte affichait des erreurs.

### Modifié
- Optimisation du menu de domaine du groupe d'onglets : Amélioration du menu de domaine du groupe d'onglets pour une meilleure organisation et convivialité.
- Optimisation du padding des onglets : Ajustement du padding des onglets pour une disposition plus épurée et visuellement attrayante.

---

## [1.0.2] - 2024-07-04

### Ajouté
- Indicateur d'onglet actif actuel : Identifiez facilement l'onglet actif avec un nouvel indicateur visuel.
- Couleur de police personnalisée : Personnalisez votre interface en définissant une couleur de police personnalisée.

### Modifié
- Optimisation de la vitesse de chargement : Amélioration de la vitesse de chargement pour une expérience utilisateur plus rapide et plus fluide.

### Paramètres par défaut
- Définir par défaut de ne pas utiliser le mode couleur : Le paramètre par défaut utilise désormais le mode couleur unique pour une apparence simplifiée.

---

## [1.0.1] - 2024-07-02

### Ajouté
- Enregistrement complet de l'historique par plage de temps : Accédez à votre historique de navigation et gérez-le avec des enregistrements détaillés triés par plage de temps.
- Mode couleur unique pour la liste : Introduction d'un mode couleur unique pour une apparence de liste simplifiée et cohérente.

### Modifié
- Timing de mise à jour de la barre de progression audio complète : Amélioration de la précision des mises à jour de la barre de progression audio pour une expérience multimédia plus fluide.
- Méthode d'acquisition des icônes de liste optimisée : Amélioration de la méthode d'acquisition des icônes de liste, ce qui permet un chargement des icônes plus rapide et plus fiable.

### Corrigé
- Correction du problème d'affichage incorrect du statut d'activation dans plusieurs fenêtres : Résolution d'un problème où le statut d'activation était affiché incorrectement lorsque plusieurs fenêtres étaient ouvertes.

---

## [1.0.0] - 2024-06-29

### Ajouté
- Basculement entre le mode clair et le mode sombre : Choisissez entre les modes d'affichage clair et sombre pour correspondre à vos préférences.
- Taille de police personnalisable : Ajustez la taille de la police pour une expérience de lecture plus confortable.
- Disposition de l'interface personnalisable : Personnalisez la disposition de l'interface en fonction de vos habitudes d'utilisation.
- Options de personnalisation : Ajoutez des arrière-plans colorés et des images de fond pour rendre votre panneau latéral unique.
- Gestion avancée des onglets : Aperçus des vignettes, options de tri et d'affichage riches, et un menu d'actions complet pour une gestion efficace des onglets.
- Fonctionnalité de recherche : Recherchez rapidement les onglets récemment fermés ou parcourez votre historique pour trouver ce dont vous avez besoin.
- Mode Image dans l'image : Passez en mode Image dans l'image de manière transparente lorsque vous changez d'onglet ou faites défiler des pages.
- Groupement automatique : Créez ou rejoignez automatiquement des groupes basés sur le même domaine pour une meilleure organisation.
- Barre de progression de lecture : Suivez votre progression de lecture en temps réel pour savoir jusqu'où vous avez lu.
- Barre de progression de lecture multimédia : Contrôlez la lecture multimédia avec des options pour avancer rapidement, revenir en arrière, régler le volume et ajuster la vitesse de lecture.
