# Hygiène numérique — Les habitudes qui protègent

## Ce qu'on entend par hygiène numérique

L'hygiène numérique, c'est l'ensemble des habitudes quotidiennes qui réduisent la surface d'attaque. Pas des outils complexes — des pratiques simples, appliquées régulièrement.

Comme l'hygiène corporelle, son efficacité ne se voit pas quand tout va bien. Elle se voit quand quelque chose ne va pas.

## Les mots de passe

**Un mot de passe par service.** La réutilisation est le problème principal. Quand une base de données est compromise quelque part, les identifiants volés sont testés automatiquement sur des dizaines d'autres services. Si le mot de passe est le même partout, un seul incident expose tout.

**Un gestionnaire de mots de passe.** Il génère et stocke des mots de passe uniques, longs et aléatoires pour chaque service. L'utilisateur n'a plus à en mémoriser qu'un seul — celui du gestionnaire. (Bitwarden, 1Password, KeePass selon les préférences et le contexte.)

**Changer les mots de passe anciens.** Un mot de passe créé il y a cinq ans sur un service potentiellement compromis depuis représente un risque. Les gestionnaires peuvent indiquer quels mots de passe sont anciens ou réutilisés.

## Les emails

**Ne pas agir sous pression.** Les emails qui demandent une action urgente sont conçus pour court-circuiter la vérification. L'urgence est une technique, pas une réalité. Prendre trente secondes pour vérifier l'expéditeur et l'URL.

**Vérifier l'adresse expéditeur complète.** Le nom affiché peut être n'importe quoi. L'adresse email derrière est plus difficile à falsifier — mais pas impossible. Le domaine est la chose à vérifier : `microsoft.com` ≠ `microsoft-secure.support`.

**Ne pas ouvrir les pièces jointes inattendues.** Surtout les formats exécutables (.exe, .js, .vbs) et les documents Office qui demandent d'activer les macros.

**Signaler plutôt que supprimer.** Un email suspect signalé à l'IT protège les collègues. Un email supprimé sans signalement laisse les autres exposés.

## Les comptes

**Activer le MFA partout où c'est possible.** En priorité sur les comptes professionnels, la messagerie, et les services financiers.

**Vérifier régulièrement les appareils et sessions actifs.** Microsoft 365, Google, et la plupart des services permettent de voir quels appareils sont connectés. Un appareil inconnu = signal d'alerte.

**Limiter les permissions accordées aux applications tierces.** Chaque application connectée à un compte email ou cloud est une surface d'attaque supplémentaire. Révoquer régulièrement les accès inutilisés.

## Ce que l'entreprise doit faire, pas l'individu

L'hygiène individuelle ne suffit pas si l'environnement n'est pas configuré correctement. La responsabilité de la sécurité n'appartient pas uniquement aux utilisateurs.

Ce qui relève de l'organisation :
- Imposer le MFA sur tous les comptes, pas le proposer
- Former les collaborateurs — pas avec un email PDF une fois par an
- Surveiller les logs et configurer des alertes
- Avoir un plan de réponse à incident documenté avant qu'il en soit besoin
- Mettre à jour les systèmes et applications régulièrement

La cybersécurité est un problème collectif résolu par des décisions individuelles et organisationnelles combinées. L'un sans l'autre ne tient pas.
