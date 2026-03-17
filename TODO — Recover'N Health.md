# ✅ TODO — Recover'N Health
> Fichier de suivi des actions à compléter avant la mise en ligne

---

## 🔴 Priorité haute — À faire avant mise en ligne

- [ ] **Remplir les mentions légales** dans le site (ouvrir la modale "Mentions légales" et remplacer tous les encadrés oranges)
  - `[PRÉNOM NOM]` → ton nom complet
  - `[ADRESSE COMPLÈTE]` → ton adresse professionnelle
  - `[NUMÉRO DE TÉLÉPHONE]`
  - `[ADRESSE EMAIL]`
  - `[SIRET à renseigner]` → une fois immatriculé·e
  - `[NOM DE L'HÉBERGEUR]` + son adresse et URL
  - `[SERVEUR N8N]` → préciser si cloud ou auto-hébergé

- [ ] **Remplacer l'URL N8N placeholder** dans `index.html`
  - Chercher : `https://TON-N8N-HOSTNAME/webhook/reservation-rnh`
  - Remplacer par l'URL réelle de ton webhook N8N

- [ ] **Remplir la page "À propos"**
  - Texte de présentation (parcours, origines antillaises/japonaises)
  - Certifications et diplômes (4 emplacements prévus)
  - Ajouter ta photo (remplacer le placeholder vert)

- [ ] **Renseigner le téléphone et l'email dans les footers** (4 footers dans le fichier)
  - Chercher : `[Numéro à renseigner]` et `[Email à renseigner]`

---

## 🟠 Priorité moyenne — Amélioration UX

- [ ] **Carte interactive Montpellier** (section "Zone d'intervention" sur la page d'accueil)
  - Actuellement : placeholder vide
  - Options recommandées :
    - **Google Maps Embed** (gratuit, simple) : générer un lien d'intégration sur maps.google.com
    - **Leaflet.js** (open-source, sans clé API) : plus personnalisable
    - **Mapbox** (design premium, nécessite une clé API gratuite)

- [ ] **Activer les mentions légales** → vérifier que les liens du footer ouvrent bien la modale

- [ ] **Tester le formulaire de réservation** une fois N8N configuré
  - Vérifier que l'email de confirmation arrive bien
  - Vérifier le récapitulatif côté N8N

---

## 🟡 Priorité basse — Sécurité & infrastructure

- [ ] **Mettre le site derrière Cloudflare** (protection DDoS gratuite)
  - Créer un compte sur cloudflare.com
  - Changer les DNS de ton domaine pour pointer vers Cloudflare
  - Activer le proxy (icône nuage orange)

- [ ] **Configurer le rate limiting sur N8N**
  - Dans ton workflow N8N, ajouter un nœud de limitation de débit
  - Exemple : max 10 requêtes / heure par IP

- [ ] **Ajouter un CAPTCHA** (optionnel mais recommandé si spam)
  - Option simple : **hCaptcha** (gratuit, respectueux RGPD)
  - Alternative : **Turnstile de Cloudflare** (invisible, très fluide)

---

## 🟢 Évolutions futures (quand base de données connectée)

- [ ] **Calendrier de disponibilités en temps réel**
  - Afficher les créneaux libres/pris dynamiquement
  - Synchronisation avec Google Calendar ou un agenda dédié

- [ ] **Espace client** (connexion, historique de séances, factures)

- [ ] **Système de paiement en ligne** (Stripe, SumUp, PayPal)
  - À mentionner dans la politique de confidentialité une fois activé

- [ ] **Avis clients dynamiques** (remplacer les témoignages figés)
  - Intégration Google Reviews ou système d'avis intégré

---

*Dernière mise à jour : Mars 2026*
