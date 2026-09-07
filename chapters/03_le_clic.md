# 03 — Le clic

La page qui s'ouvre ressemble à la page de connexion Microsoft. Fond blanc, logo en haut, champ email, champ mot de passe. L'URL dans la barre du navigateur : `https://login.microsoft-secure.support/oauth`.

Sarah tape son adresse email. Elle tape son mot de passe. Elle clique sur **Se connecter**.

Un message apparaît : "Connexion réussie. Vous allez être redirigé vers votre boîte de réception." Quelques secondes plus tard, Outlook s'ouvre normalement — elle était déjà connectée, la session n'avait pas expiré.

Elle hausse les épaules. Ferme l'onglet. Reprend ses emails.

---

**Ce qui vient de se passer**

Sarah a entré ses identifiants sur une page qu'elle ne contrôle pas. Ces identifiants ont été envoyés en temps réel à un serveur distant. Pas à Microsoft.

La redirection vers Outlook réel est intentionnelle. Elle évite que Sarah se pose des questions. Du point de vue de l'utilisatrice, rien d'anormal ne s'est produit. Elle est connectée. Tout fonctionne.

Le mot de passe est désormais connu de l'attaquant. Il va maintenant tester si ce même mot de passe fonctionne ailleurs — LinkedIn, Gmail, d'autres services professionnels. C'est ce qu'on appelle le **credential stuffing** : tester des identifiants volés sur d'autres plateformes, parce que les gens réutilisent leurs mots de passe.

Sarah utilise `Veritas2020!` sur LinkedIn aussi. Et sur son compte Gmail personnel.

→ `fiches/phishing.md` — les pages de phishing et comment les identifier
→ `fiches/mfa.md` — pourquoi un mot de passe seul ne suffit plus
