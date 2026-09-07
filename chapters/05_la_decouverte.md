# 05 — La découverte

Trois jours plus tard.

Le comptable externe rappelle pour confirmer le changement de RIB. Il tombe sur la directrice administrative, qui n'a pas été informée d'un changement de coordonnées bancaires. Elles vérifient ensemble avec l'employée. l'employée n'a pas envoyé cet email.

La directrice appelle le DSI. Le DSI se connecte à la console d'administration Microsoft 365. Il voit :

- Une connexion depuis une IP roumaine le 14 mars à 9h23.
- Trente-deux emails lus dans la foulée.
- Une règle de transfert automatique créée à 9h41.
- Un email envoyé depuis le compte de l'employée à 10h02.

Trois jours de boîte copiée en temps réel vers l'extérieur.

---

**Ce qui a retardé la découverte**

Personne n'a vu d'anomalie pendant trois jours parce que personne ne regardait. Pas d'alerte sur la connexion depuis un pays inhabituel. Pas de notification à l'employée d'une nouvelle connexion sur son compte. Pas de surveillance des règles de transfert créées dans les boîtes des collaborateurs.

Les traces étaient là dès le premier jour. Les logs Microsoft les enregistrent automatiquement. Mais des logs que personne ne lit ne servent à rien.

La détection a eu lieu par accident — un coup de téléphone de vérification, pas un système d'alerte.

Ce n'est pas rare. La durée moyenne entre une compromission et sa découverte est de plusieurs semaines dans les PME. Pendant ce temps, l'attaquant opère.

→ `fiches/detection.md` — surveiller une boîte, lire les logs, mettre en place des alertes
