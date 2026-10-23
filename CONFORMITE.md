# Mise en conformité légale — RM Sites (23/10/2026)

Cas vérifié dans le code : page de présentation de Raphaël Mata (RM Sites), future micro-entreprise libérale (pas encore immatriculée), création de sites pour des professionnels. Rien n'est vendu en ligne, aucun formulaire : contact par téléphone. Hébergement actuel : GitHub Pages, IONOS prévu sur rm-sites.fr. `devis.html` est un outil interne (non relié, noindex).

Ce document n'est pas un avis juridique.

## Fichiers créés ou modifiés

| Fichier | Changement |
|---|---|
| `index.html` | Nouvelle vue CGV (`#cgv`) avec formulaire de rétractation, section confidentialité complétée (`#confidentialite`), hébergeur réel, liens du pied de page, comparatif de prix sans marque nommée, contrastes (or et mode sombre), repères pour lecteurs d'écran, Open Graph, canonique, données structurées |
| `devis.html` | Mention des CGV et du droit de rétractation des petites entreprises |
| `robots.txt` | Toujours fermé avant le lancement, avec la version à mettre au lancement |
| `llms.txt`, `sitemap.xml` | Nouveaux : pour moteurs de recherche et assistants IA |

## Point par point

1. **Mentions légales — s'applique.** Déjà complètes sur le principe. Hébergeur corrigé : le site est aujourd'hui chez GitHub, pas chez IONOS. Restent : adresse, SIRET, e-mail, date.
2. **Confidentialité — s'applique (peu de données).** Aucun formulaire. Traitements : échanges par téléphone ou e-mail, journaux de l'hébergeur (GitHub, États-Unis, pendant la préparation). Section renforcée et ancrée (`#confidentialite`), lien dans le pied de page.
3. **Cookies — pas de bandeau.** Aucun cookie, polices déjà hébergées sur le site, aucune requête vers un autre site (vérifié).
4. **CGV — s'applique.** Tu vends des prestations à des professionnels : les CGV doivent être communiquées avec chaque devis. Créées à partir de ton offre réelle : devis, acompte 50 %, pénalités de retard et indemnité de 40 €, délais 7 et 14 jours, corrections, propriété du site après paiement complet, domaine au nom du client, suivi 19 €/mois et sans suivi 99 €/an, responsabilité, clause de sous-traitance RGPD (article 28), formulaire de rétractation.
5. **CGU — non applicable.**
6. **Médiateur — non applicable** : tes clients sont des professionnels, pas des consommateurs.
7. **Formulaires — non applicable** : aucun formulaire public. Le futur bouton « Écrire » (mailto) ne collecte rien sur le site.
8. **Services tiers.** Aucun chargé à l'ouverture. Les liens vers les démos claude.ai ne sont que des liens.
9. **Accessibilité (recommandée).** Corrigé : or des petits textes foncé en mode clair (#86672D, contraste 4,7:1 au lieu de 3,95:1) ; en mode sombre, les liens et boutons verts étaient presque invisibles (contraste 1,2:1) : nouvelle couleur de texte vert clair ; bandeau du haut et barre mobile nommés. Contrôle automatique : plus aucune erreur sur les 4 vues, en clair et en sombre. `devis.html` (outil interne) non corrigé.
10. **Agents IA.** llms.txt (offre et prix), sitemap.xml, canonique rm-sites.fr, Open Graph, données structurées « ProfessionalService ». robots.txt reste fermé jusqu'au lancement ; la version à mettre est écrite dans le fichier.
11. **Contenu :**
    - **Comparatif de prix** : citait « un site Wix » nommément ; remplacé par « un abonnement à un constructeur de site en ligne ». Les fourchettes agence / indépendant restent des repères datés, à garder seulement si tu peux montrer d'où elles viennent.
    - **Réalisations** : les démos sont marquées fictives (bien). Mais les liens mènent à des pages claude.ai **privées** : un visiteur tombe sur une page d'erreur. À rendre partageables, ou remplacer par les vrais sites avec l'accord des clients.
12. **Coordonnées.** Cohérentes (nom, statut, téléphone). Pas encore d'e-mail ni de SIRET.
13. **Autres risques :**
    - **Droit de rétractation des petites entreprises** : en démarchant les commerces chez eux, un client de 5 salariés au plus peut annuler sous 14 jours. Sans information écrite, ce délai peut s'allonger jusqu'à 12 mois. C'est maintenant dans les CGV et sur le devis : remets le formulaire de rétractation avec chaque devis signé, et ne commence le travail avant 14 jours que si le client le demande par écrit.
    - **Sous-traitance RGPD** : quand tu héberges un site avec formulaire (comme Aqua Beauté), tu traites les données des visiteurs de ton client. La clause est dans les CGV (article 12).
    - **Copie claude.ai de la page** (artifact « Devanture ») : elle n'a pas ces changements. À mettre à jour ou à ne plus diffuser.
    - **Pas de devis officiel ni de facture avant le SIRET.**

## À faire par un humain

- [ ] Après la micro-entreprise : SIRET, adresse, e-mail, date (mentions légales, CGV, devis).
- [x] Choix des CGV tranchés le 23/10 : suivi payé chaque mois ou 12 mois d'avance ; après 12 mois, mois par mois avec un mois de préavis ; tribunaux selon le droit commun.
- [ ] Rendre les démos partageables ou les remplacer.
- [ ] Au lancement : robots.txt ouvert (modèle dans le fichier), retirer `noindex`, mettre à jour l'hébergeur (IONOS) et retirer le paragraphe GitHub.
- [ ] Relecture des CGV par la CCI ou un juriste avant le premier client.

## Jugé non applicable (contredis-moi si besoin)

- **Bandeau cookies** : aucun traceur.
- **Médiateur de la consommation** : clients professionnels uniquement.
- **CGU et formulaires** : pas de compte, pas de formulaire.
- **Déclaration d'accessibilité** : micro-entreprise.
