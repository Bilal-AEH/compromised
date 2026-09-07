# 06 — La réponse

Il est 14h37. Le DSI a confirmé la compromission. La directrice convoque une réunion d'urgence. Il faut agir — mais dans quel ordre ?

Sans plan de réponse préparé, les premières décisions sont improvisées. Et l'improvisation sous pression génère des erreurs.

---

**Ce qui a été fait — dans le bon ordre, cette fois**

**1. Contenir**
Priorité immédiate : couper l'accès de l'attaquant. Le DSI réinitialise le mot de passe du compte de Sarah et active le MFA en urgence. Il supprime la règle de transfert automatique. Il révoque toutes les sessions actives sur le compte.

L'attaquant perd son accès à 15h04 — soit 77 heures après avoir obtenu les identifiants.

**2. Évaluer**
Qu'est-ce qui a fuité ? Le DSI exporte les logs de connexion et l'historique des emails envoyés depuis le compte compromis. Il identifie : les emails lus, les pièces jointes téléchargées, les contacts externes qui ont reçu des messages de l'attaquant.

**3. Notifier**
Le comptable externe est prévenu. Le virement vers le faux RIB n'a pas encore été effectué — il est bloqué à temps. Les autres contacts qui ont reçu des emails suspects pendant les 77 heures sont alertés.

**4. Corriger**
L'IT déploie le MFA sur l'ensemble des comptes de l'entreprise — pas seulement celui de Sarah. Audit des règles de transfert sur toutes les boîtes. Formation phishing planifiée pour l'ensemble des collaborateurs.

**5. Documenter**
Un rapport d'incident est rédigé. Il décrit la chronologie, les données exposées, les actions prises, les mesures correctives. Il sera utile si une déclaration CNIL est nécessaire.

---

**Ce que ça coûte sans préparation**

77 heures de compromission. Des emails confidentiels copiés. Un virement frauduleux évité de justesse. Deux jours de travail mobilisés pour la réponse. Une formation phishing qui aurait coûté une heure par collaborateur si elle avait eu lieu avant.

La réponse à incident est un processus. Quand il n'est pas préparé, il se passe mal même quand l'issue est favorable.

→ `fiches/detection.md` — réponse à incident, étapes et priorités
