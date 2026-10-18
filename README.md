# ResaColis / Toulouse Maroc

Base de projet pour le service de **collecte et d'expédition de colis de Toulouse vers le Maroc**.

> **État : prototype statique.** Il n'existe à ce stade ni compte client, ni réservation en ligne, ni paiement, ni suivi de colis, ni base de données. Ne pas présenter ce site comme un service de réservation opérationnel.

## Démarrer

Ouvrir `index.html` dans un navigateur. Aucun logiciel à installer. Pour un hébergement statique, publier le contenu du dépôt à sa racine.

## Arborescence

- `index.html` : page de présentation et formulaire local de préparation de demande.
- `assets/styles.css` : mise en forme responsive.
- `assets/app.js` : validation et génération d'un récapitulatif copiable ; aucun envoi automatique.
- `docs/parcours-client.md` : parcours et règles à confirmer avant production.
- `docs/modele-donnees.md` : modèle cible et précautions de confidentialité.
- `examples/demande.example.json` : exemple **fictif** de demande.
- `.gitignore` : exclusions Git.

## Utilisation

1. Le client consulte les informations générales.
2. Il prépare un récapitulatif de demande (ville, nombre de colis, poids estimé).
3. Il copie ce texte pour contacter l'équipe par son canal habituel.
4. L'équipe confirme **manuellement** l'éligibilité, le tarif, la collecte et le départ.

Aucune donnée saisie n'est envoyée ni sauvegardée par le site.

## Avant mise en production

- Valider la liste des villes desservies, les zones de collecte, les horaires et conditions de transport.
- Faire valider les mentions légales, politique de confidentialité, conditions générales et processus de réclamation.
- Mettre en place un véritable backend sécurisé avant d'accepter des réservations et données personnelles.
- Définir les règles de colis interdits, déclaration de contenu, douanes, assurance et preuve de remise.
- Tester l'affichage mobile et l'accessibilité.

## Organisation

Ce dépôt contient une base technique initiale et non un outil logistique prêt à l'exploitation. Les contributions doivent éviter d'ajouter des données réelles de clients, des secrets ou des clés API dans Git.
