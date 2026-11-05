| ID | Date | Découverte | Constat / preuve | Reco | Statut | Décision |
|---|---|---|---|---|---|---|
| NB-D1 | 05/11 | Clic gauche du bouton edge n'ouvre pas l'urlbar flottante | Lecture du code : `window.URLBar20` est undefined — `URLBar20` est une const locale de l'IIFE d'URLBar-2.0, jamais exposée sur `window` → le contrat appelait du vide (optional chaining silencieux) | Exposer `window.URLBar20 = URLBar20` dans urlbar-2.0.uc.js (1 ligne) | 🆕 | |
| NB-D2 | 05/11 | Superpositions de son au clic du bouton (notamment middle) | Double `playClick()` : le handler mousedown button-0 jouait avant son check de bouton, puis le handler middle rejouait | Déplacer `playClick()` après les checks de bouton dans chaque handler | 🆕 | |
