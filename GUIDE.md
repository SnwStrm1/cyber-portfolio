# Prendre en main ton portfolio

## 1. Ouvrir et personnaliser

Décompresse le ZIP. Ouvre le dossier dans VS Code puis ouvre index.html dans ton navigateur. Modifie une phrase de l’intro, enregistre et actualise le navigateur. Ensuite, essaie de changer la valeur de --accent en haut de style.css pour voir où la couleur est réutilisée. Les polices utilisent celles déjà disponibles sur l’appareil.

Le pseudo est SnwStrm1, avec un lien vers le compte GitHub du même nom. Si tu choisis un autre nom d’affichage, modifie les titres, l’en-tête et le pied de page sur les deux pages. Vérifie également ce que ton profil GitHub affiche publiquement avant de le relier au site.

Relis le retour Bpifrance dans tes mots. Le texte est un brouillon de mémoire. Ajoute uniquement les étapes dont tu es sûre. Si tu retrouves la consigne ou une capture, vérifie les règles de publication du CTF et retire les identifiants des personnes avant de la partager.

## 2. Expliquer ton code

- index.html contient la page d’accueil. nav regroupe les liens, section regroupe une rubrique et article contient un travail qui peut se lire seul.
- href="#write-ups" amène le navigateur à l’élément id="write-ups". Sur la page du CTF, ../index.html#write-ups remonte au dossier parent et revient à cette rubrique.
- style.css donne aux deux pages les mêmes couleurs et espacements. :root contient les couleurs réutilisées. .wrap borne la largeur du contenu. flex-wrap permet aux liens de revenir à la ligne quand l’écran rétrécit.
- Les chemins relatifs continuent de fonctionner quand GitHub sert le site sous /cyber-portfolio/. ../style.css remonte d’un dossier depuis un write-up pour retrouver la feuille de style.

En entretien, ouvre les fichiers et montre le trajet entre le lien de l’accueil, la page du write-up et la feuille de style. Ensuite, raconte un changement que tu as fait et comment tu l’as vérifié.

## 3. Ajouter un write-up

Duplique write-ups/bpifrance-osint.html dans le même dossier. Donne-lui un nom comme mon-challenge.html. Change le titre de l’onglet, la description, le h1 et le contenu de l’article. Dans index.html, copie l’article de la rubrique Write-ups et change le lien vers write-ups/mon-challenge.html. Teste l’aller et le retour.

Pour écrire, réponds à quatre questions avec tes propres mots.

1. Qu’est-ce qu’on te demandait et quels indices avais-tu au départ ?
2. Quelle piste as-tu testée et qu’est-ce qui t’a fait changer de direction ou poursuivre ?
3. Quel élément a confirmé le résultat ? Qu’as-tu fait toi-même et qu’a fait l’équipe ?
4. Qu’est-ce que tu ferais de nouveau lors d’un autre challenge ?

Pour Bpifrance, commence avec une phrase que tu peux vérifier de mémoire. Par exemple, explique ce qui t’a fait reconnaître que la chaîne correspondait à la recherche, si tu t’en souviens.

## 4. Détailler un projet

La carte Security Toolkit présente le prototype. Pour approfondir, prends le module que tu peux reprendre et expliquer. Par exemple, montre le parcours d’une ligne de log fictive depuis l’entrée jusqu’à la sortie. Dans le README du projet, indique le besoin, le format d’entrée, comment lancer le script, un exemple de résultat et une limite réellement observée. Ajoute le lien du dépôt à la carte quand il est prêt. Si un module est encore difficile à expliquer, tu peux commencer par un TP que tu maîtrises déjà.

Pour ajouter une deuxième carte, duplique l’article de la rubrique Projets dans index.html. Donne-lui un titre descriptif et une phrase sur ce que tu as fait. Quand tu auras un premier travail CTI à montrer, pars d’un rapport public sur une campagne et explique ce que tu as extrait des sources, ce que tu as recoupé et ce qui reste incertain. Cite tes sources.

## 5. Construire le cas avant-vente Novatech

Novatech est une PME fictive de 150 salariés. Commence par cinq questions de découverte client sur le parc, les outils existants, le traitement des alertes, le budget et le risque prioritaire. Écris les réponses que tu imagines pour le scénario et présente-les comme des hypothèses.

Compare EDR, XDR et SIEM en fonction de ces réponses. Choisis une approche, explique ce qui motive ton choix et prépare une présentation de trois minutes pour une direction non technique. Ajoute un schéma simple et, quand le dossier est prêt, crée sa page sur le modèle du write-up puis ajoute le lien sur l’accueil.

Pour le projet CTI, garde le rapport source et une trace de tes recoupements. Si tu proposes une piste de détection, précise les logs nécessaires et indique si tu as pu la tester dans un lab.

## 6. Publier sur GitHub Pages

Si Pages est déjà configuré, copie les fichiers HTML et CSS de cette version dans le dépôt existant, puis vérifie le rendu en ouvrant index.html. Fais un commit et pousse sur la branche qui publie le site.

1. Ouvre ton dépôt existant cyber-portfolio et repère sa branche principale. Place index.html, style.css et le dossier write-ups à côté du README. Garde ce guide à portée de main pour les prochaines modifications.
2. Fais un commit, par exemple « Ajouter la première version du portfolio ». Dans GitHub, ouvre Settings → Pages.
3. Sous Build and deployment, sélectionne Deploy from a branch, puis main (ou la branche sur laquelle tu as mis tes fichiers) et / (root). Clique sur Save.
4. Quand le déploiement est terminé, utilise Visit site dans Settings → Pages. Vérifie le lien du write-up, le retour vers la rubrique et le lien GitHub. Réduis aussi la largeur de la fenêtre pour tester l’affichage mobile.

Documentation : https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
