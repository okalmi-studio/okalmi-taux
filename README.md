# okalmi-taux

Taux et seuils officiels de la micro-entreprise (France), au format JSON, lus automatiquement par le **Livre des recettes OKALMI** à chaque ouverture.

- Fichier : [`taux.json`](taux.json)
- Contenu : année, taux de cotisations (vente de marchandises, prestations BIC, BNC, Cipav), taux ACRE selon la date de début d'activité, CFP, taxe pour frais de chambre consulaire, plafonds de chiffre d'affaires, seuils de franchise de TVA, versement libératoire, abattements forfaitaires, date de dernière mise à jour et liens des sources officielles.
- Sources : urssaf.fr, autoentrepreneur.urssaf.fr, entreprendre.service-public.gouv.fr, impots.gouv.fr, economie.gouv.fr (liens dans le fichier).

Le livret fonctionne aussi sans connexion : il garde alors les derniers taux connus.

## Mise à jour annuelle (5 lignes)

1. Vérifier les nouveaux chiffres sur urssaf.fr, service-public.fr et impots.gouv.fr (en janvier, puis après toute réforme).
2. Ouvrir `taux.json` sur GitHub → crayon « Modifier » → corriger les valeurs, l'`annee`, la `derniereMiseAJour` (AAAA-MM-JJ) et les sources.
3. Vérifier que le JSON reste valide (pas de virgule en trop ; un aperçu « Preview » sans erreur).
4. « Commit changes » : GitHub Pages republie le fichier en 1 à 2 minutes.
5. Ouvrir le livret avec internet : le bandeau doit afficher « Taux à jour (mise à jour du JJ/MM/AAAA) » avec la nouvelle date.
