# Sources consultées — TEST AI SCRAPING #1

## Moteur de scraping
- **Firecrawl Open Source** (self-hosted)
- Déploiement: Docker Compose sur VPS (localhost:3002)
- Images: ghcr.io/firecrawl/firecrawl:latest, playwright-service, nuq-postgres, redis, rabbitmq
- Méthode: API v1/scrape avec moteur Playwright
- Limitation: Sans Fire-engine cloud, certains sites anti-bot (Cloudflare) restent bloqués

## Sites scrapés avec Firecrawl
| Festival | URL | Statut Firecrawl | Données extraites |
|----------|-----|-----------------|-------------------|
| Paléo Festival Nyon | https://yeah.paleo.ch/fr/contact | ✅ Succès | +41 22 365 10 10, adresse Nyon |
| Montreux Jazz Festival | https://www.montreuxjazzfestival.com/fr/festival/faq/ | ✅ Succès | info@mjf.ch, ticketinfo@mjf.ch, +41 900 800 800 |
| Foire de Genève (Palexpo) | https://www.palexpo.ch/fr/contact | ✅ Succès | info@palexpo.ch, +41 22 761 11 11 |
| Fête du Blé et du Pain | https://www.feteduble.ch | ✅ Succès | info@fetedubleetdupain.ch |
| Festival de la Bâtie | https://www.batie.ch | ✅ Succès | Info générale |
| Musilac | https://www.musilac.com | ✅ Succès (404 apparent) | Emails partiels |
| Printemps de Pérouges | https://printempsdeperouges.fr | ✅ Succès | Pas de contacts directs |
| Blues aux Remparts | https://www.paysvoironnais.com/agenda/blues-aux-remparts | ✅ Succès | Pas de contacts directs |
| Fête du Lac Annecy | https://www.lac-annecy.com | ✅ Succès | Pas de contacts directs |
| Annemasse (Noctibules) | https://www.annemasse.fr/culture | ✅ Succès | Pas de contacts directs |

## Sites bloqués / inaccessibles
| Festival | URL | Raison |
|----------|-----|--------|
| Fêtes de Genève | https://www.fetesdegeneve.ch | Certificat SSL invalide |
| Fête de la Bière Genève | https://www.bieres-geneve.ch | Bloqué |
| Festival de la Cité Lausanne | festivaldelacite.ch | Domaine en vente |

## Contacts non vérifiés (basés sur éditions précédentes / annuaires)
Les festivals marqués "⚠️ Partiel" dans le JSON ont des contacts basés sur les éditions précédentes.
Une vérification téléphonique est recommandée avant prospection.

## Commandes Firecrawl utilisées
```bash
# Scrape simple
curl -X POST http://localhost:3002/v1/scrape \
  -H 'Content-Type: application/json' \
  -d '{"url": "https://example.com", "formats": ["markdown"]}'
```