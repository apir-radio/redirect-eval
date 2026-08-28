# eval.apir-radio.fr

Deux redirections minimales GitHub Pages :

- `https://eval.apir-radio.fr/formulaire` vers le Google Form d’évaluation ;
- `https://eval.apir-radio.fr/resultats` vers le Google Sheets privé des résultats.

La racine `https://eval.apir-radio.fr` redirige vers `/formulaire` pour préserver l’ancien lien.

## Changer les destinations

- Formulaire : modifier [`formulaire/destination.js`](formulaire/destination.js).
- Résultats : modifier [`resultats/destination.js`](resultats/destination.js).

Dans chaque fichier, remplacer uniquement l’URL entre guillemets puis valider le commit. La nouvelle destination sera publiée automatiquement. Il n’y a rien à changer dans le DNS, le domaine personnalisé ou les autres fichiers.

## Configuration

- Domaine : `eval.apir-radio.fr`
- Publication : branche `main`, dossier `/ (root)`
- DNS : `CNAME eval → apir-radio.github.io.`
- Indexation : désactivée par les balises `robots`
- Authentification supplémentaire : aucune ; les droits du Sheet restent gérés par Google

Le fichier `CNAME` doit rester présent. Le fichier `.nojekyll` désactive tout traitement Jekyll inutile.
