# TEST AI SCRAPING #1

## Festivals dans un rayon de 100km de La Plonge S'adapte
**226 rue du Jura, Neydens (74160), Haute-Savoie, France**

**Période :** 19 juin 2026 → 30 septembre 2026
**Minimum participants :** 1000+
**Cible :** Festivals avec verre à laver (buvettes, bars, restauration)

## 🔥 Firecrawl Open Source — Self-hosted
Firecrawl a été déployé en self-hosted sur ce VPS via Docker Compose :
- **Endpoint :** http://localhost:3002
- **Moteur :** Playwright (scraping JavaScript)
- **Containers :** api, playwright-service, redis, rabbitmq, nuq-postgres
- **Succès :** 10/15 sites scrapés avec succès

## Résultats par statut Firecrawl
| Statut | Nombre |
|--------|--------|
| ✅ Scrapé avec contacts | 5 festivals |
| ✅ Scrapé (sans contacts directs) | 5 festivals |
| ⚠️ Contacts via autres sources | 3 festivals |
| ❌ Bloqué / inaccessible | 2 festivals |

## Top 5 prospects prioritaires
1. **Paléo Festival Nyon** — 40km, 21-26 juillet, 230k festivaliers
   📞 +41 22 365 10 10
2. **Montreux Jazz Festival** — 60km, 3-18 juillet, 200k+
   📧 info@mjf.ch | 📞 +41 21 966 44 44
3. **Fêtes de Genève** — 15km, 1-15 août, 100k+
   📧 fetes@ville-ge.ch | 📞 +41 22 418 44 00
4. **Foire de Genève (Palexpo)** — 15km, 20 août-5 sept, 50-100k
   📧 info@palexpo.ch | 📞 +41 22 761 11 11
5. **Fête du Blé et du Pain** — 70km, 1-3 août, 20-50k
   📧 info@fetedubleetdupain.ch

## Fichiers
- `festivals_complet.json` — Données structurées (15 festivals, 1000+ participants)
- `festivals_contacts.csv` — Export CSV pour prospection
- `sources.md` — URLs, méthodologie Firecrawl, statuts

---

*Généré le 12 juin 2026 — Donna, Sovereign Executive Shadow*
*Tool: Firecrawl Open Source (self-hosted) + vérifications manuelles*