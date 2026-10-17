# Retours à faire à l'association — École de l'engagement

Document de suivi des points à clarifier ou à obtenir auprès de l'association pour finaliser le site.

---

## Priorité haute

### Linktree
- [ ] Identifier qui a accès aux comptes de l'asso (email utilisé)
- [ ] Créer le compte Linktree avec le bon email : https://linktr.ee
- [ ] Renseigner tous les réseaux et liens dans le Linktree une fois le compte créé

### HelloAsso
- [ ] Confirmer que la collecte promo-3 est bien active : https://www.helloasso.com/associations/ecole-de-l-engagement/collectes/promo-3
- [ ] Si une nouvelle collecte est ouverte pour une promo suivante, mettre à jour le lien dans `index.html` (section Don)

### Email de contact
- [ ] Confirmer que `contact@ecole-de-lengagement.fr` est actif et relevé régulièrement
- [ ] Si non, remplacer par l'email réellement utilisé

---

## Priorité moyenne

### Réseaux sociaux
- [ ] Vérifier si un compte Twitter / X existe — si oui, communiquer l'URL pour l'ajouter au footer
- [ ] Vérifier si d'autres réseaux sont à ajouter (LinkedIn, YouTube, etc.)

### Domaine
- [ ] Confirmer le domaine souhaité (ex: `ecole-de-lengagement.fr`)
- [ ] Configurer les DNS pour pointer vers Vercel (instructions dans le README)
- [ ] Vérifier que le domaine est bien renouvelé et actif
- [ ] Une fois le domaine actif : remplacer `ecole-de-lengagement.vercel.app` par le domaine définitif dans `index.html` (canonical, og:url, og:image, JSON-LD), `mentions-legales.html`, `confidentialite.html`, `sitemap.xml` et `robots.txt`

### Mentions légales / confidentialité
- [ ] Pages créées (`mentions-legales.html`, `confidentialite.html`) mais contiennent des placeholders à compléter avec l'association : adresse du siège social, n° SIREN/RNA, nom du directeur de publication, durée de conservation des données de candidature

---

## Priorité basse

### Contenu à mettre à jour
- [ ] Informations sur la prochaine promotion (dates d'ouverture des candidatures, numéro de promo)
- [ ] Photos des promotions suivantes a ajouter dans `images/`
- [ ] Intervenants et programme mis a jour si nécessaire

### Pages manquantes
- [ ] Mentions légales (lien présent dans le footer mais page inexistante)
- [ ] Politique de confidentialité (idem)

---

## Notes

- Le site est déployable sur Vercel dès maintenant (voir README)
- Les modifications sont a pousser sur la branche `main` du repo : https://github.com/kevingaga/EcoleEngagement
- Tout push sur `main` déclenche un redéploiement automatique
