# La Juste Part

Des outils simples et sourcés pour que les plus grandes fortunes paient leur juste part.

> « La Juste Part » est un nom provisoire. Pour le changer, remplacez-le dans `index.html`, `reponses.html` et `quart-dheure.html` (en-tête, pied de page et balise `<title>` de l'accueil).

## Contenu

| Page | Rôle |
|---|---|
| `index.html` | Accueil : les chiffres clés et les outils |
| `reponses.html` | **Ils disent… Vous répondez.** Neuf arguments contre la taxation des plus grandes fortunes, chacun avec une réponse courte à copier, le détail, ce qui est vrai dans l'argument et les sources. Chaque fiche a son lien direct (par exemple `reponses.html#exil`). |
| `quart-dheure.html` | **Leur quart d'heure.** Le temps qu'il faut à un foyer milliardaire pour gagner votre revenu annuel, le mécanisme des holdings, une carte à partager et un message pour son député. |
| `site.css` | Styles communs |

Le site est entièrement statique : HTML, CSS et JavaScript, sans dépendance ni étape de compilation. Seule la police Archivo est chargée depuis Google Fonts.

## Mettre en ligne avec GitHub Pages

1. Créez un dépôt public sur GitHub (par exemple `la-juste-part`).
2. Envoyez-y le contenu de ce dossier, à la racine du dépôt (bouton **Add file → Upload files**, ou `git push`).
3. Dans le dépôt : **Settings → Pages → Build and deployment**, choisissez **Deploy from a branch**, branche `main`, dossier `/ (root)`, puis **Save**.
4. Après une à deux minutes, le site est en ligne à l'adresse `https://<votre-compte>.github.io/la-juste-part/`.

Le fichier `.nojekyll` évite que GitHub transforme les fichiers : laissez-le en place.

## Ajouter ou corriger un argument

Les fiches sont dans le tableau `ARGS` en haut du script de `reponses.html`. Chaque fiche contient :

- `id` : l'ancre du lien direct (lettres, chiffres, tirets) ;
- `tag` : le mot court affiché dans les raccourcis ;
- `say` : l'argument, dans sa forme la plus forte ;
- `short` : la réponse courte, qui doit tenir dans un commentaire ;
- `detail` : la réponse chiffrée ;
- `truth` : ce qui est vrai dans l'argument (ne jamais la supprimer : c'est ce qui rend la réponse crédible) ;
- `sources` : une liste de paires `[titre, adresse]`. Le bouton « Copier la réponse » ajoute la première source.

Règle : aucun chiffre sans source publique, et quand les économistes ne sont pas d'accord, la fiche le dit.

## Sources principales

- Institut des politiques publiques, note n° 92, « Quels impôts les milliardaires paient-ils ? » (2023, données 2016)
- Conseil d'analyse économique, Focus n° 118 sur l'émigration fiscale (2025)
- France Stratégie, comité d'évaluation des réformes de la fiscalité du capital, rapport final (2023)
- Sondage Ifop pour le Parti socialiste (septembre 2025)

La liste complète figure sur chaque fiche.
