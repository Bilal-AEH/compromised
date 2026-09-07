# Phishing — Anatomie d'une attaque par email

## Ce que c'est

Le phishing est une technique d'attaque qui consiste à usurper l'identité d'un expéditeur de confiance pour pousser la victime à effectuer une action — cliquer un lien, entrer des identifiants, ouvrir une pièce jointe.

C'est l'attaque la plus répandue dans le monde. Pas parce qu'elle est sophistiquée — parce qu'elle fonctionne.

## Anatomie d'un email de phishing

Un email de phishing bien construit reproduit les éléments visuels et textuels d'un email légitime :

- **Logo et charte graphique** copiés depuis le site officiel
- **Ton et formulation** calqués sur les communications habituelles de l'expéditeur
- **Urgence artificielle** : "votre compte sera suspendu", "action requise sous 24h"
- **Appel à l'action unique** : un seul bouton, un seul lien, pas le temps de réfléchir

Ce qui trahit un email de phishing, quand on prend le temps de regarder :

| Élément | Légitime | Phishing |
|---|---|---|
| Domaine expéditeur | `@microsoft.com` | `@microsoft-secure.support` |
| URL du lien | `login.microsoft.com` | `login.microsoft-secure.support` |
| Personnalisation | Prénom, contexte | Générique |
| Pression temporelle | Rare | Systématique |

## La page de phishing

Le lien mène vers une page qui copie l'interface de connexion du service visé. Quand la victime entre ses identifiants, ils sont envoyés au serveur de l'attaquant — puis la page redirige vers le vrai service pour éviter l'éveil des soupçons.

L'URL est le signal le plus fiable : vérifier le domaine avant d'entrer quoi que ce soit.

## Les variantes

- **Spear phishing** : ciblé sur une personne précise, avec des éléments personnels (prénom, entreprise, interlocuteur connu). Taux de succès bien plus élevé.
- **Whaling** : ciblé sur des dirigeants.
- **Smishing** : même principe, par SMS.
- **Vishing** : par téléphone.

## Ce qui protège

1. Vérifier l'adresse expéditeur complète — pas le nom affiché, l'adresse réelle.
2. Ne jamais cliquer un lien depuis un email urgent — aller directement sur le site.
3. Vérifier l'URL avant d'entrer des identifiants.
4. Signaler les emails suspects à l'IT plutôt que les supprimer.
