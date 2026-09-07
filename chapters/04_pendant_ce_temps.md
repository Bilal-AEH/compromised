# 04 — Pendant ce temps

9h23. Sarah est en réunion.

L'attaquant se connecte à sa boîte Outlook depuis une adresse IP en Roumanie. Microsoft n'a pas bloqué la connexion — le bon mot de passe a été fourni, et il n'y a pas d'authentification à deux facteurs sur le compte.

Ce qu'il fait en premier : il lit. Pas au hasard — il cherche des patterns. Les emails avec des clients, les échanges avec la direction, les accès partagés mentionnés dans les conversations. Il cherche à comprendre qui est Sarah dans l'organisation, ce à quoi elle a accès, et ce qu'il peut extraire ou exploiter.

Il trouve plusieurs choses utiles. Des échanges avec un comptable externe mentionnant des coordonnées bancaires. Des documents RH en pièce jointe. Une conversation avec le DSI sur un accès VPN en cours de configuration.

À 9h41, il configure une règle de transfert automatique : tous les emails reçus par Sarah sont désormais copiés en temps réel vers une adresse externe qu'il contrôle. La règle est discrète — elle ne supprime pas les emails originaux, elle les copie. Sarah continuera à tout recevoir normalement.

À 10h02, il envoie depuis la boîte de Sarah un email au comptable externe. Objet : "Changement de RIB pour virement fournisseur". Il joint un RIB falsifié. L'email vient de l'adresse légitime de Sarah, avec sa signature habituelle.

Sarah est toujours en réunion.

---

**Ce que ça révèle**

Une boîte email compromise n'est pas seulement une perte de données personnelles. C'est une position à l'intérieur du réseau de confiance de la victime — ses collègues, ses clients, ses fournisseurs. L'attaquant bénéficie de la réputation de Sarah. Ses emails sont crus parce qu'ils viennent d'elle.

La règle de transfert est un mécanisme de persistance : même si le mot de passe est changé plus tard, les emails continueront à fuir jusqu'à ce que la règle soit découverte et supprimée.

→ `fiches/detection.md` — les traces qu'une compromission laisse et comment les trouver
