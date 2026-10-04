# Steam Market Mapping

Étude de marché Steam réalisée le 4 octobre 2026 pour cadrer un jeu premium Steam visant une sortie 2027-2028, pensé pour le clip et l'anecdote factory.

**Rapport en ligne :** https://mathieucabot.github.io/SteamMarketMapping/

## Contenu

- `index.html` : le rapport complet, servi par GitHub Pages à l'adresse ci-dessus. Grille comparative de 17 familles de jeux (cinq axes notés, triable en cliquant les en-têtes), fiches par genre, zones recommandées, les deux lentilles de design, limites et sources. S'ouvre aussi en local dans un navigateur.
- `donnees/macro.md` : cadre macro Steam 2025-2026 (volumes, médianes, conversion wishlists, Next Fest, prix, algorithme) et dossier clipping (cas documentés, écosystème, conversion vue vers vente).
- `donnees/g-friendslop-party-bluff.md` : coop horreur à physique, party physique, déduction sociale.
- `donnees/g-colony-sandbox-automation.md` : colony sim, sandbox systémique et immersive sim, automation.
- `donnees/g-survival-extraction-competitif.md` : survival crafting coop, extraction PvPvE, sports physique et horreur asymétrique.
- `donnees/g-roguelite-deckbuilder-jobsim.md` : roguelite action et bullet heaven, roguelike deckbuilder, job sims.
- `donnees/gl_*.json` : extractions brutes de l'API publique Gamalytic (`api.gamalytic.com/steam-games/list`) pour les six tags témoins, cohortes 2024-2026, relevées le 4 octobre 2026. `gl_summary.json` contient les médianes et percentiles calculés à partir de ces extractions.

Les données des genres témoins (tactique, narratif court, cozy, metroidvania) sont intégrées directement dans le rapport.

## Conventions

Chaque chiffre est daté. « Sourcé » désigne un chiffre publié par l'éditeur, Valve ou un média citant une source officielle. « Estimation » désigne un modèle tiers (Gamalytic, VG Insights, Raijin, SteamPulse, Boxleiter), fondé sur le nombre d'avis Steam. Ces modèles sous-estiment les hits à bas prix et surestiment les hits chers.

## Ce qui manque

Volumes de sorties par tag et par année pour les genres non témoins (SteamDB et Gamalytic bloquent l'accès automatisé ; l'API publique Gamalytic a toutefois répondu et peut servir à compléter), Google Trends, vues TikTok chiffrées, conversion clip vers vente quantifiée.

## Lentilles de design

Deux jeux de statements testables sur playtest filmé, détaillés dans le rapport :

- Lentille A, le clip : ce que voit un spectateur étranger en 15 à 60 secondes.
- Lentille B, l'anecdote factory : ce que le joueur raconte le lendemain.

Les piliers (hook, core experience, identité esthétique) restent au-dessus des deux lentilles.

## Publication

Le site est servi depuis la branche `main`, dossier racine, via GitHub Pages. Le fichier `.nojekyll` désactive le traitement Jekyll pour que les fichiers soient servis tels quels.
