# Sources consultées

## Sites officiels vérifiés
| Festival | URL | Statut |
|----------|-----|--------|
| Montreux Jazz Festival | https://www.montreuxjazzfestival.com | ✅ Accessible |
| Paléo Festival Nyon | https://yeah.paleo.ch | ✅ Accessible |
| Fêtes de Genève | https://www.fetesdegeneve.ch | ❌ Certificat SSL invalide |
| Musilac | https://www.musilac.com | ❌ 404 |
| Printemps de Pérouges | https://printempsdeperouges.fr | ⚠️ Non accessible via curl |
| Festival de la Cité | https://www.festivaldelacite.ch | ❌ Domaine en vente |
| Festival d'Annecy | https://www.annecyfestival.com | ✅ Accessible (animation, pas de verre) |
| Blues aux Remparts | https://www.bluesauxremparts.com | ⚠️ Non accessible via curl |
| Fête du Blé et du Pain | https://www.feteduble.ch | ⚠️ Non vérifié |
| Fête de la Bâtie | https://www.batie.ch | ⚠️ Non vérifié |

## Outils utilisés
- **Firecrawl** (open source) — SDK Python installé (firecrawl-py v4.28.2)
- **Browser** — Navigation Chromium pour les sites accessibles
- **curl** — Requêtes HTTP pour les sites sans JS lourd
- **DuckDuckGo Search** — Recherche textuelle (rate-limité sur VPS)

## Limitations
- Plusieurs sites bloquent les requêtes automatisées (Cloudflare, CAPTCHA)
- Les festivals suisses sont mieux documentés que les petits festivals français
- Les contacts téléphoniques et emails des petits festivals (comités des fêtes) nécessitent une prospection téléphonique directe
- Les dates 2026 des festivals traditionnels (fêtes du boudin, de la pomme, etc.) ne sont pas encore publiées