# Formation CSS

Projet d'exemple réalisé dans le cadre de l'apprentissage du CSS.

Pendant les blocs du cours, vous travaillez sur de petites pages
indépendantes, rangées dans `cours/` : pour chaque bloc, une démonstration à
suivre et un exercice à réaliser. Le **site**, quatre pages écrites en HTML
et livrées sans aucune mise en forme, vous l'habillerez pendant les travaux
pratiques, en fin de parcours.

## Ce qui vous est fourni

| Fichier                            | Description                                                                                                                                                                                                                                                             |
| ---------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Les quatre pages `.html`           | Le site terminé côté structure. **Vous n'avez pas à les modifier**, sauf quand une consigne vous le demande explicitement.                                                                                                                                              |
| `css/style.css`                    | Volontairement vide. C'est le fichier que vous écrirez pendant les travaux pratiques.                                                                                                                                                                                   |
| `cours/`                           | Le travail des blocs, un dossier par bloc (`01-selecteurs/`…). Chacun contient `demonstration/`, la page à habiller en suivant la fiche, et `exo/`, l'exercice : la page, sa maquette et son guide de style. Dans les deux cas, vous n'écrivez que la feuille de style. |
| `assets/img/` et `assets/favicon/` | Les images et le favicon utilisés par les pages.                                                                                                                                                                                                                        |
| `.vscode/`                         | Les réglages de l'éditeur et les extensions conseillées. VS Code vous proposera de les installer à l'ouverture du dossier.                                                                                                                                              |
| `.prettierignore`                  | Empêche l'éditeur de remettre votre CSS en forme à votre place.                                                                                                                                                                                                         |

> **Il n'y a pas de `base.css` dans ce projet, et c'est voulu.**
> Ceux qui viennent du cours de HTML avaient une feuille de style fournie, là
> pour rendre leur travail lisible. Elle a disparu : vos pages sont nues, et
> tout ce qui apparaîtra à l'écran désormais viendra de vous.

## Prérequis

- [Visual Studio Code](https://code.visualstudio.com/)
- Un compte [GitHub](https://github.com/)
- [Git](https://git-scm.com/downloads) : facultatif. Le projet se récupère
  sans lui, il ne sert qu'à enregistrer votre avancement et à publier :
  voir « Enregistrer votre travail » plus bas

Les extensions VS Code ne sont pas à chercher : **le projet les propose
lui-même** à la première ouverture du dossier. Acceptez, elles sont toutes
gratuites.

## Démarrer

### 1. Récupérer le projet

Le projet de départ se télécharge d'un bloc :

**[Télécharger le projet de départ](https://github.com/aarnow/formation-css/archive/refs/heads/starter.zip)**

Décompressez l'archive où vous voulez travailler. Le dossier obtenu s'appelle
`formation-css-starter`, vous pouvez le renommer.

> **Ni fork ni clone.** Le dépôt porte aussi le site terminé et les corrigés,
> un par bloc. En le copiant entier, vous auriez les réponses avant les
> questions. L'archive ne contient que le départ.

### 2. Ouvrir le projet

Dans VS Code : **Fichier → Ouvrir le dossier**, puis choisissez le dossier que
vous venez de décompresser.

**Le dossier, pas un fichier.** C'est la seule façon pour que les chemins vers
`css/` et `assets/` se comportent comme prévu, et pour que l'éditeur applique
les réglages du projet.

À la première ouverture, VS Code propose d'installer les extensions
recommandées. Acceptez.

### 3. Voir votre page

L'extension d'aperçu installée avec le projet sert votre site sur un vrai
serveur local et recharge la page à chaque enregistrement.

- Clic droit sur `index.html` → **Open with Live Server**.
- Le site s'ouvre à l'adresse `http://127.0.0.1:5501`.
- Chaque enregistrement recharge la page toute seule : gardez le navigateur
  à côté de l'éditeur.

Gardez aussi l'inspecteur ouvert, touche `F12`, onglet **Éléments**. C'est là
que vous verrez quelles règles s'appliquent vraiment à un élément, et
lesquelles sont ignorées.

### 4. Enregistrer votre travail

Votre dossier ne vit que sur votre disque : pas de retour en arrière si vous
cassez quelque chose, pas de sauvegarde ailleurs. **Faites des copies du
dossier de temps en temps**, en particulier avant une grosse modification.

Rien ne vous empêche de lui donner un dépôt dès maintenant, vous y déposerez
votre avancement au fur et à mesure.

Sur GitHub, bouton **+** en haut à droite → **New repository**. Nommez-le,
cochez **Public**, créez-le. Puis, selon que vous avez Git ou non :

**Avec Git**, une fois dans le dossier du projet :

```bash
git init
git remote add origin https://github.com/VOTRE-PSEUDO/VOTRE-DEPOT.git
git add .
git commit -m "Bloc 01 : les sélecteurs"
git push -u origin main
```

Les fois suivantes, trois commandes suffisent, toujours les mêmes :

```bash
git add .
git commit -m "Bloc 02 : la boîte et la remise à zéro"
git push
```

**Sans Git**, tout passe par l'interface :

1. Sur la page du dépôt vide : **uploading an existing file**.
2. Glissez-y le contenu de votre dossier, vos pages, `css/`, `assets/`.
   Les dossiers sont conservés. Validez avec **Commit changes**.
3. Ensuite, pour mettre à jour : **Add file → Upload files**, et remplacez
   les fichiers modifiés.

C'est là que Git vous manquera : ce qu'une commande fait en une seconde vous
prendra quelques clics à chaque fois.

> Les fichiers `.vscode/` et `.prettierignore` ne servent qu'à votre éditeur.
> S'ils ne montent pas, ça n'a aucune conséquence sur le site en ligne.

## Suivi du cours

Les blocs, les exercices et les QCM sont sur la page de parcours :

**https://support-formation.netlify.app/**

Vous y trouverez aussi les annexes à garder ouvertes pendant tout le cours.

Votre progression y est enregistrée **dans votre navigateur, sur votre poste**.
Elle ne remonte à personne et elle est perdue si vous changez de machine ou
de navigateur.
