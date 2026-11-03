# Reflections — Logistics dashboards

## Reflection 1 — Which stakeholder will disagree most? (before building)

Je pense que c'est le responsable des opérations / coûts qui sera en désaccord avec les deux autres. Le responsable RSE et le responsable stratégie veulent tous les deux réduire les distances, donc ils seront sans doute d'accord pour ouvrir un nouvel entrepôt, alors que pour le responsable coûts, un entrepôt en plus c'est un loyer, du personnel et du stock en plus.

## Reflection 2 — Which assumption would I least want to defend to a client?

Celle que j'aurais le plus de mal à défendre, c'est la demande estimée à partir de la population (50 tonnes/an pour 1000 habitants). Le facteur CO2 (0,10 kg/t.km) est dans une fourchette officielle publiée (ministère, ADEME), donc je peux citer une source. Les coûts ne sont pas sourcés non plus, mais ils ne servent qu'au dashboard coût, alors que la demande inventée sert aux trois : tout le CO2, tous les coûts et le choix du réseau en dépendent. Et une grande ville ne commande pas forcément plus de marchandises qu'une ville industrielle plus petite.

## Reflection 3 — Two KPIs pointing to different actions for the same warehouse

Pour Lille, les dashboards CO2 et coût disent 0 kg de CO2 et 0 € de transport : aucune autre ville ne lui est rattachée, il ne coûte que 466 196 € de stockage, donc on aurait envie de le fermer. Mais le KPI réseau dit l'inverse : fermer Lille fait passer la distance moyenne pondérée de 168,04 à 174,43 km, parce que ses 233 098 habitants devraient alors être livrés depuis Paris. Un KPI pousse à fermer, l'autre à garder.

## Reflection 4 — Would I trust the #1-ranked CO2 route?

Le trajet n°1 est Marseille ← Lyon, avec 1 212 t de CO2 par an sur 277,6 km. Je ne le recommanderais pas tel quel pour de la consolidation : il est en tête surtout parce que Marseille est la 2e plus grande ville (873 076 habitants, donc beaucoup de tonnes estimées), pas parce que le trajet est mal organisé. En plus, Marseille est justement un candidat pour un nouvel entrepôt : la vraie solution n'est peut-être pas de consolider ce trajet mais de le supprimer en ouvrant Marseille. Sinon, c'est l'axe de la vallée du Rhône, où il y a déjà du fret ferroviaire, donc un report vers le rail serait à étudier. Et la distance est à vol d'oiseau, la vraie distance par la route est plus longue.

## Reflection 5 — Which lever first for the highest-cost warehouse?

Lyon est l'entrepôt le plus cher : 13 476 013 €/an, soit 69,21 €/tonne contre 50,91 € pour Paris. Le stockage est la plus grosse part (7 788 952 €), mais dans ce modèle il est juste proportionnel au tonnage (40 €/t), donc on ne peut pas le réduire sans livrer moins. Je jouerais sur le transport : 5 687 061 €, soit environ 29 €/tonne pour Lyon contre environ 11 €/tonne pour Paris, parce que Lyon livre des villes très loin (Toulouse à 360 km, Bordeaux à 436 km).

## Reflection 6 — My recommendation, the caveat, and Reflection 1 revisited

J'ouvrirais Marseille : la distance moyenne pondérée passe de 168,04 à 115,03 km (-32 %), mieux que Bordeaux (139,89 km), et Marseille reprend Toulouse, Nice, Montpellier et Toulon, ce qui supprime aussi le trajet n°1 en CO2. Je ne fermerais pas Lille (174,43 km, c'est pire). L'avertissement sur le capex ne change pas mon choix, mais je le présenterais comme une première étape : il faudrait chiffrer l'ouverture et vérifier que les économies de transport la remboursent. Pour la réflexion 1, je me suis à moitié trompé : dans les chiffres, les trois dashboards vont plutôt dans le même sens (moins de distance = moins de CO2 et moins de transport). Le désaccord du responsable coûts n'apparaîtrait qu'en ajoutant le coût d'ouverture, qui n'est pas dans le modèle. Le vrai conflit que je n'avais pas vu, c'est Lille, qui paraît inutile en CO2 et en coût mais utile pour le réseau.

## Reflection 7 — My fourth chart (Step 15)

J'ai ajouté un graphique au dashboard CO2 : les kg de CO2 par tonne livrée pour chaque entrepôt, avec la moyenne du réseau. La page dit qu'elle aide à trouver l'entrepôt le moins efficace par tonne, mais aucun des deux graphiques ne répondait à ça : ils montrent des totaux, qui dépendent surtout de la taille des villes. Résultat : Lyon est à 24,34 kg/t, bien au-dessus de la moyenne (16,8), Paris à 9,09 et Lille à 0. J'ai choisi des barres triées parce que c'est un ratio à comparer entre 3 entrepôts, pas une part d'un total (donc pas de camembert), et pas une carte puisque la question n'est pas « où » mais « lequel ».

