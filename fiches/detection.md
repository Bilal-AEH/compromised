# Détection et réponse à incident

## Les traces qu'une compromission laisse

Une attaque sur une boîte email laisse des traces dans les logs — à condition que quelqu'un les lise.

**Logs de connexion Microsoft 365**
Chaque connexion est enregistrée : adresse IP, pays, date et heure, succès ou échec, type d'appareil. Une connexion depuis un pays inhabituel, depuis un nouvel appareil, ou à une heure inhabituelle est un signal.

**Règles de boîte de réception**
Les règles de transfert, de suppression automatique ou de déplacement sont enregistrées. Toute règle créée récemment et non reconnue par l'utilisateur est suspecte.

**Emails envoyés**
L'historique des emails envoyés depuis un compte compromis révèle ce que l'attaquant a fait pendant son accès.

**Tentatives de connexion échouées**
Plusieurs échecs suivis d'un succès = tentative de bruteforce ou de credential stuffing. C'est visible dans les logs avant même la connexion réussie.

## Ce qu'on surveille en pratique

Dans une entreprise qui a mis en place une surveillance minimale :

- **Alerte sur connexion depuis un pays non habituel** pour les comptes sensibles
- **Alerte sur création de règle de transfert** dans n'importe quelle boîte
- **Rapport hebdomadaire** des nouvelles connexions et appareils
- **Audit régulier** des comptes administrateurs et des permissions

Ces alertes ne nécessitent pas d'outil complexe sur Microsoft 365 — elles sont configurables dans la console d'administration.

## Réponse à incident — dans l'ordre

Quand une compromission est confirmée :

**1. Contenir** — couper l'accès de l'attaquant en priorité
- Réinitialiser le mot de passe du compte compromis
- Activer le MFA si ce n'est pas déjà fait
- Révoquer toutes les sessions actives
- Supprimer les règles de transfert ou de suppression créées par l'attaquant

**2. Évaluer** — comprendre l'étendue de la compromission
- Quelles données ont été lues ou téléchargées ?
- Quels emails ont été envoyés depuis le compte ?
- D'autres comptes sont-ils concernés ?

**3. Notifier** — prévenir les personnes impactées
- Contacts qui ont reçu des emails de l'attaquant
- Partenaires ou clients potentiellement visés par des demandes frauduleuses
- CNIL si des données personnelles ont été exposées (obligation légale en France sous 72h)

**4. Corriger** — appliquer les mesures qui auraient évité l'incident
- MFA sur tous les comptes
- Formation phishing
- Surveillance des logs

**5. Documenter** — constituer un rapport d'incident
- Chronologie précise
- Données exposées
- Actions prises
- Leçons tirées

## La règle des 77 heures

Dans le cas de l'employée, l'attaquant a opéré 77 heures avant la découverte. La durée moyenne de non-détection dans les PME est de plusieurs semaines. Chaque heure supplémentaire augmente le volume de données exposées et complique la réponse.

La surveillance proactive réduit ce délai. La détection accidentelle — un coup de téléphone — n'est pas une stratégie.
