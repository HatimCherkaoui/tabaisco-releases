# Politique de confidentialité — Tabaisco

Dernière mise à jour : 31 mars 2026

## Résumé

Tabaisco ne collecte, ne stocke et ne transmet aucune donnée personnelle
à ses propres serveurs. L'extension n'a aucun serveur propre.

## Données collectées

Tabaisco ne collecte aucune donnée personnelle.

## Données stockées localement

Les préférences de l'utilisateur (moteur de recherche, thème, source
d'actualités, ligue sportive, unité de température, sujets d'intérêt,
localisation manuelle, indicateur de don masqué)
sont sauvegardées exclusivement dans `chrome.storage.sync`, le stockage
intégré de Chrome. Ces données ne quittent jamais les appareils de
l'utilisateur sauf pour se synchroniser entre ses propres appareils via
le compte Google Chrome de l'utilisateur, conformément à la politique
de confidentialité de Google.

## Géolocalisation

La géolocalisation est utilisée uniquement pour afficher la météo locale.
Les coordonnées sont transmises directement à l'API Open-Meteo
(open-meteo.com) pour obtenir la température et les conditions
météorologiques. Elles ne sont ni stockées ni envoyées à l'éditeur de
l'extension.

## Services tiers

L'extension contacte les services suivants au nom de l'utilisateur :

| Service                 | Domaine                       | Usage                                  |
| ----------------------- | ----------------------------- | -------------------------------------- |
| Open-Meteo              | `open-meteo.com`              | Météo locale, sans compte ni clé       |
| OpenStreetMap Nominatim | `nominatim.openstreetmap.org` | Géocodage inverse du nom de ville      |
| BBC News                | `feeds.bbci.co.uk`            | Flux RSS public d'actualités           |
| Google News             | `news.google.com`             | Flux RSS public d'actualités           |
| Hacker News             | `hnrss.org`                   | Flux RSS public d'actualités           |
| ESPN                    | `site.api.espn.com`           | Scores sportifs, API publique sans clé |
| PayPal                  | `paypal.me`, `paypal.com`     | Destination du bouton de don optionnel |

Chacun de ces services est soumis à sa propre politique de confidentialité.
Tabaisco n'intercepte, ne journalise ni ne modifie les données échangées
avec ces services.

## Sécurité du code

L'extension déclare une Politique de Sécurité du Contenu (CSP) explicite
dans son manifeste : `script-src 'self'; object-src 'self'`. Aucun script
extérieur ni inline ne peut s'exécuter. L'instruction `eval()` et
`new Function()` ne sont pas utilisées (vérifié par les tests automatisés
à chaque build).

## Publicité et pistage

L'extension ne contient aucun script publicitaire, aucun tracker,
aucune balise analytique, aucun pixel de suivi.

## Enfants

L'extension n'est pas destinée aux enfants de moins de 13 ans et ne
collecte aucune donnée les concernant.

## Modifications

Toute modification de cette politique sera annoncée via une mise à jour
de l'extension sur le Chrome Web Store.

## Contact

Pour toute question : cherkaouihatim@gmail.com
