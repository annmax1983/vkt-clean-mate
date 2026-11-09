# VKT CleanMate

[English](../README.md) | [中文](README_zh.md) | [日本語](README_ja.md) | [Deutsch](README_de.md) | [Español](README_es.md) | Français

Voir ce qui va être supprimé avant de le supprimer. Les sites de confiance restent intacts, et au passage vous saurez où passe votre temps.

> Chrome · Edge · Firefox · Manifest V3 · Permissions minimales · 100 % local · Sans analytique

Fait partie de la boîte à outils de confidentialité [VKT](https://www.annmax1983.com/).

---

## Pourquoi VKT CleanMate ?

La plupart des nettoyeurs sont un gros bouton « tout effacer ». C’est précisément pour cela qu’on n’ose pas les activer : un clic et toutes les sessions disparaissent. Pire, avant de cliquer, vous ne savez pas s’il va toucher 3 sites ou 3000.

VKT CleanMate sépare la décision de l’action.

| Ce que font les autres nettoyeurs | Le prix |
|---|---|
| Un interrupteur qui efface tout | Un mauvais clic et les sessions, les cookies et l’historique des téléchargements ont disparu |
| Une boîte de confirmation sans chiffres | Impossible de savoir si cela concerne 3 ou 3000 sites avant de valider |
| Des règles par site cachées derrière un champ de regex | Personne ne les écrit, donc le mode « sûr » n’est jamais utilisé |

| Ce que fait VKT CleanMate | Le résultat |
|---|---|
| **Une feuille d’aperçu à chaque exécution manuelle** | Des chiffres réels lus dans le navigateur : sites trouvés, entrées d’historique, cookies, types actifs, fenêtre de conservation |
| **La version gratuite ne peut pas tout effacer** | Aucun chemin vers la suppression accidentelle — par conception, pas par avertissement |
| **Deux listes en directions opposées** | Liste de nettoyage (« seulement ceux-là », gratuite) et liste de protection (« jamais ceux-là », gratuite elle aussi, respectée dans les deux modes) |
| **Les limites sont écrites** | Dans l’interface et dans ce README, plutôt que découvertes par un examinateur |

En une phrase : **voir ce qui part avant de supprimer, et savoir ensuite où est passé le temps.**

---

## Fonctionnalités

### 🆓 Gratuit, pour toujours

| Fonction | Ce qu’elle fait |
|---|---|
| Aperçu | Sites trouvés, entrées d’historique, cookies, types de données et conservation avant toute suppression |
| Mode ciblé | Ne nettoie que les domaines de votre liste de nettoyage. Entrées illimitées |
| Neuf types de données | Historique, cache, cookies, historique des téléchargements, données de formulaires, stockage local, IndexedDB, service workers et mots de passe enregistrés, chacun avec son interrupteur |
| Conservation | Garder le dernier jour / 3 jours / 7 jours / 30 jours, ou tout |
| Cinq déclencheurs | Au démarrage, à la fermeture, toutes les N minutes, chaque jour à une heure fixe, après N minutes d’inactivité |
| Portée par déclencheur | Par exemple historique + cache toutes les quelques heures, nettoyage profond avec cookies à la fermeture |
| Raccourcis | `Alt+Shift+C` nettoyer maintenant · `Alt+Shift+X` nettoyer puis fermer tous les onglets et fenêtres |
| Report | Repousser la prochaine exécution automatique d’une heure |
| Notifications | Un résumé du résultat après chaque exécution |
| Six langues | English, 简体中文, 日本語, Deutsch, Español, Français |

### ⭐ Pro (licence requise)

| Fonction | Ce qu’elle fait |
|---|---|
| Mode complet | Tout effacer sauf votre liste de protection |
| Liste de protection | Les domaines à ne jamais toucher ; en cas de conflit, la protection l’emporte |
| Empreinte de concentration | Temps de concentration réel par domaine, répartition sur 24 heures, classement, suggestions de nettoyage |
| Export CSV | L’empreinte en CSV, une ligne par domaine |

Une licence couvre deux navigateurs. Les fonctions gratuites continuent de fonctionner après expiration.

---

## Ce qu’il sait faire, et ce qu’il ne sait pas faire

### ✅ Il sait

- Effacer l’historique, le cache, les cookies, les téléchargements, les données de formulaires, le stockage local, IndexedDB, les service workers et les mots de passe, dans n’importe quelle combinaison.
- Limiter un nettoyage aux domaines que vous avez nommés, sous-domaines compris, sans écrire d’expression régulière.
- Sauter les domaines que vous protégez, en mode complet.
- Nettoyer selon un planning, avec une portée de données différente par déclencheur.
- Dire exactement ce qui a été supprimé, à chaque fois.

### ❌ Il ne sait pas

- Vider les caches DNS, les journaux du routeur, les enregistrements du fournisseur d’accès ou les logs serveur. Ce n’est pas sur votre appareil.
- Restaurer un historique supprimé. Chromium n’offre à aucune extension d’API pour réécrire l’historique.
- Nettoyer les données d’un autre navigateur, d’un autre profil ou d’une copie synchronisée sur un autre appareil.
- Limiter l’historique, les téléchargements, les données de formulaires ou les mots de passe à un seul site. Le navigateur ne l’expose pas ; ces quatre types ne sont filtrés qu’en mode complet, et l’interface le dit à côté de la case.
- Garantir le déclencheur « à la fermeture du navigateur ». C’est du meilleur effort : un plantage, un redémarrage forcé ou une coupure de courant peuvent perdre cette exécution.
- Nettoyer ce qui n’a jamais été stocké. Une page seulement lue dans une fenêtre privée ne laisse rien.
- Remplacer un VPN ni vous défendre contre une surveillance au niveau du réseau. C’est un outil en libre-service pour votre propre navigateur sur votre propre appareil.

---

## Aperçu

| Capture | Contenu |
|---|---|
| [`01-popup.png`](../screenshots/01-popup.png) | Panneau de la barre d’outils, site courant déjà dans la liste de nettoyage |
| [`02-preview.png`](../screenshots/02-preview.png) | La feuille de confirmation « Before cleaning » |
| [`03-cleaning.png`](../screenshots/03-cleaning.png) | Réglages : mode, types de données, conservation, déclencheurs |
| [`04-lists.png`](../screenshots/04-lists.png) | Réglages : liste de nettoyage et liste de protection |
| [`05-footprint.png`](../screenshots/05-footprint.png) | Page d’empreinte : totaux, répartition horaire, classement |

---

## Navigateurs compatibles

| Navigateur | État |
|---|---|
| Chrome 116+ (bureau) | ✅ Compatible |
| Microsoft Edge 116+ (bureau) | ✅ Compatible |
| Autres navigateurs Chromium avec MV3 | ✅ Devrait fonctionner |
| Firefox (bureau) | ✅ Compatible |
| Mobile / tablette | ❌ Non compatible : il n’y a pas de barre d’outils |
| Fenêtres privées | ⚠️ Rien à nettoyer : les données sont jetées à la fermeture |

---

## Installation

**Depuis la boutique :** Chrome Web Store, Microsoft Edge Add-ons ou Firefox Add-ons (AMO) → « Ajouter à Chrome » → épinglez l’icône dans la barre d’outils.

**Depuis les sources :**

```bash
npm install          # terser, uniquement pour le build
npm run build        # dist/ + publish/cleanmate-v<version>.zip
```

Puis `chrome://extensions` → Mode développeur → Charger l’extension non empaquetée → ce dossier (ou le `dist/` décompressé).

---

## Utilisation

### Première fois

Ouvrez le panneau et cliquez sur **Nettoyer maintenant**. Comme le mode par défaut est Ciblé et que la liste de nettoyage est vide, rien ne se passe encore : c’est justement le but. Ajoutez d’abord un domaine, dans le panneau pour le site courant ou dans l’onglet **Lists**.

### Remplir la liste de nettoyage

- Dans le panneau : **Ajouter le site courant** enregistre le domaine que vous regardez.
- Dans l’onglet Lists : tapez `example.com` puis Add. Les sous-domaines sont couverts automatiquement, `www.` est retiré pour vous.
- Sur la page d’empreinte (Pro) : les suggestions « mérite un nettoyage » et chaque ligne du classement ont un bouton qui ajoute le domaine.

### Configurer les exécutions automatiques

Dans l’onglet **Cleaning**, chacun des cinq déclencheurs a son interrupteur. En dessous, un menu déroulant fixe la portée de données de ce déclencheur : `global` suit les cases au-dessus, toute autre valeur limite cette exécution à un préréglage (historique + cache, cookies + cache, tout, etc.).

Un point de départ raisonnable : historique + cache toutes les 6 heures, tout à la fermeture du navigateur, et démarrage comme inactivité laissés éteints jusqu’à être sûr d’en vouloir.

### Raccourcis

| Touches | Action |
|---|---|
| `Alt+Shift+C` | Nettoyer maintenant avec les réglages actuels |
| `Alt+Shift+X` | Nettoyer maintenant, puis fermer tous les onglets et fenêtres |

Les deux se modifient dans `chrome://extensions/shortcuts`.

---

## Comment ça marche

1. Un déclencheur se met en route, ou vous cliquez sur Nettoyer maintenant.
2. Le service worker d’arrière-plan détermine la portée : votre liste de nettoyage en mode ciblé, tout moins la liste de protection en mode complet.
3. Lors d’une exécution manuelle, il compte ce qui serait touché — sites, entrées d’historique, cookies — et affiche la feuille d’aperçu. **Rien n’a encore été supprimé.**
4. Après validation, chaque type sélectionné est supprimé via `chrome.browsingData`, par lots de 50 origines au maximum. Une exécution programmée (intervalle, quotidienne, inactivité, à la fermeture) saute la feuille : elle applique vos règles et notifie le résultat.
5. Les règles de domaine sont d’abord converties en origines réelles : `browsingData` accepte des origines (`https://example.com`) et non des noms d’hôtes nus, et n’étend pas les sous-domaines de lui-même.
6. Une notification rend compte du résultat, l’horodatage de l’exécution est enregistré, et la feuille reste accessible depuis le panneau.

Un détail d’implémentation utile à connaître : `browsingData` n’honore `origins` que pour le cache, les cookies, le stockage local, IndexedDB, les service workers et les systèmes de fichiers. L’historique, les téléchargements, les données de formulaires et les mots de passe ignorent complètement cette liste : lorsque ces types sont cochés, l’exécution porte sur tout le profil. L’extension l’écrit dans l’interface au lieu de le cacher.

---

## Questions fréquentes

**Le nettoyage supprime-t-il mes favoris ?**
Non. Les favoris ne font pas partie de `browsingData` et aucun code de l’extension n’y touche.

**Supprimer les cookies va-t-il me déconnecter partout ?**
En mode ciblé, uniquement des domaines de votre liste. C’est pourquoi la version gratuite ne fonctionne qu’en mode ciblé : un effacement complet est une décision payante, prise volontairement, liste de protection en main.

**Puis-je nettoyer l’historique d’un seul site ?**
Oui. Cela nécessite la permission optionnelle `history`, demandée au moment où vous prévisualisez ou nettoyez l’historique par site, pas à l’installation.

**Cela supprime-t-il les mots de passe synchronisés avec mon compte Google ?**
Si vous cochez **Mots de passe enregistrés**, le navigateur supprime le stockage local des mots de passe, et un profil connecté peut propager cette suppression. Ce type est désactivé par défaut et signalé en rouge dans l’interface précisément pour cette raison. Laissez-le décoché sauf si vous le voulez vraiment.

**Cela fonctionne-t-il dans les fenêtres privées ?**
Une fenêtre privée jette ses données à la fermeture, il ne reste donc rien à nettoyer. L’extension n’a pas besoin d’accéder aux fenêtres privées.

**Le déclencheur « à la fermeture » ne s’est pas exécuté.**
C’est du meilleur effort. Il se déclenche quand le nombre de fenêtres atteint zéro ; si le navigateur se ferme en pleine tâche, le nettoyage se termine quelques secondes après le démarrage suivant. Un plantage, un redémarrage forcé ou une coupure de courant perdent cette exécution.

**Nettoie-t-il d’autres navigateurs ou d’autres profils ?**
Non. Un profil, un navigateur, cet appareil.

**Pourquoi seul le mode complet est-il payant ?**
Parce que « tout effacer » est la seule opération capable de supprimer des sessions dont vous avez encore besoin, et la seule qu’un nettoyeur ciblé ne peut structurellement pas faire. Tout le reste — la liste de protection comme l’empreinte de focus — fonctionne sans licence. Pro vend l’opération risquée et l’enregistrement au long cours, pas le droit de regarder ses propres données.

---

## Confidentialité

Pas d’analytique, pas de télémétrie, pas de publicité, pas de compte. L’extension ne lit pas le contenu des pages, n’enregistre pas les frappes et ne construit aucun profil. Les réglages vivent dans `chrome.storage.local`. L’empreinte de concentration, si elle est activée, stocke domaines, durées, nombres de visites et une répartition horaire sur une fenêtre glissante de 30 jours : ni URL ni titres. La seule requête réseau de toute l’extension est la vérification de licence auprès de `api.annmax1983.com`, et seulement si vous collez une clé.

**[📄 Politique de confidentialité complète](../privacy-policy.html)**

### Autorisations

| Autorisation | Pourquoi |
|---|---|
| `browsingData` | Supprimer les types de données choisis |
| `storage` | Conserver réglages et empreinte optionnelle sur votre appareil |
| `alarms` | Planifications, plus un battement par minute pour le chronomètre de concentration |
| `tabs` | Connaître le domaine courant et agir sur l’onglet visible |
| `windows` | Détecter la fermeture de la dernière fenêtre — base du déclencheur « à la fermeture » |
| `idle` | Le déclencheur optionnel « après inactivité » |
| `notifications` | Le résumé du résultat après une exécution |
| `history` *(optionnel)* | Uniquement pour prévisualiser ou nettoyer l’historique par site |
| `cookies` *(optionnel)* | Uniquement pour nettoyer les cookies par site |
| `api.annmax1983.com` | Activation et validation de licence uniquement |

Ces deux autorisations optionnelles expliquent pourquoi une installation neuve n’affiche pas l’avertissement rouge « lire votre historique de navigation ».

---

## Mention de copyright

VKT CleanMate est un outil indépendant. Il n’est affilié ni à Google, ni à Microsoft, ni à aucun éditeur de navigateur. Chrome, Edge et Firefox sont des marques de leurs propriétaires respectifs.

L’extension supprime des données via les API du navigateur lui-même. Elle ne modifie pas le navigateur, ne touche pas aux fichiers système et n’installe rien en dehors de son propre dossier.

---

## ❤️ Soutenir

**[👉 Obtenir une licence](https://annmax1983.com/extensions/cleanmate)** · **[☕ Offrez-moi un café](https://ko-fi.com/annmax?ref=vkt-clean-mate)** · [Code sur GitHub](https://github.com/annmax1983/vkt-clean-mate) · [Site officiel](https://annmax1983.com/)

---

## Avis sur le code source

> ⚠️ **Ce dépôt sert uniquement à la présentation du projet — le code source complet n'y est pas publié.** Il ne contient que la documentation d'utilisation, les notes de version et les informations d'assistance de l'extension.

> 📥 **Téléchargement et installation uniquement depuis les boutiques officielles :** Chrome Web Store · Microsoft Edge Add-ons · Modules complémentaires Firefox (AMO). Aucun installateur hors ligne n'est distribué ici.

---

## Licence

Copyright © 2026 VKT CleanMate. All rights reserved.

Ce logiciel est propriétaire et à code fermé. Sans autorisation écrite préalable de l'auteur, la décompilation, l'ingénierie inverse, le crackage, la modification, le reconditionnement, la redistribution ou la revente du logiciel (en tout ou en partie) sont strictement interdites.
