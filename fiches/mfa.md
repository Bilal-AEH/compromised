# MFA — Authentification multi-facteurs

## Le problème du mot de passe seul

Un mot de passe est un secret partagé entre vous et le service. Si quelqu'un d'autre obtient ce secret — par phishing, par fuite de base de données, par réutilisation sur un site compromis — il a exactement le même accès que vous.

Le mot de passe seul ne distingue pas son propriétaire légitime d'un attaquant qui le connaît.

## Ce que le MFA change

Le MFA (Multi-Factor Authentication) exige plusieurs preuves d'identité simultanées, issues de catégories différentes :

- **Ce que vous savez** : mot de passe, code PIN
- **Ce que vous avez** : téléphone, clé physique (YubiKey), carte
- **Ce que vous êtes** : empreinte digitale, reconnaissance faciale

Un attaquant qui a volé votre mot de passe ne peut pas se connecter s'il lui manque le deuxième facteur — généralement votre téléphone.

## Les formes de MFA

**Code par SMS** — un code à 6 chiffres envoyé par SMS. Simple à déployer. Vulnérable au SIM swapping (usurpation de numéro de téléphone) — acceptable pour la plupart des usages, pas pour les comptes très sensibles.

**Application d'authentification** (Authenticator, Authy) — génère un code qui change toutes les 30 secondes. Plus sécurisé que le SMS, indépendant du réseau téléphonique.

**Clé physique** (YubiKey, clé FIDO2) — périphérique USB ou NFC à brancher. Résiste au phishing : la clé vérifie cryptographiquement qu'elle communique bien avec le vrai site. Standard le plus solide pour les comptes critiques.

**Notification push** — l'application demande une confirmation sur le téléphone. Pratique, mais vulnérable au **MFA fatigue** : bombarder la victime de demandes jusqu'à ce qu'elle valide par erreur ou par lassitude.

## Pourquoi il n'est pas activé par défaut

Le MFA ajoute une étape. Les services le proposent, rarement le forcent — par crainte de perdre des utilisateurs. Dans les entreprises, il est souvent optionnel jusqu'à ce qu'un incident pousse à le rendre obligatoire.

## Ce que ça change concrètement

Dans le cas de Sarah : si le MFA avait été activé, l'attaquant aurait eu le mot de passe correct et n'aurait pas pu se connecter. Microsoft aurait envoyé une demande de confirmation sur le téléphone de Sarah. Elle l'aurait vue, ne l'aurait pas approuvée, et l'IT aurait pu être alerté d'une tentative de connexion suspecte.

Un mot de passe volé aurait été inutile.
