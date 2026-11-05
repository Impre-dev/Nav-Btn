# Session du 05/11 (création Nav-Btn + fusion Phase A/B)

## État courant
Nav-Btn v1.2.0 — clone NavBtn porteur du bouton fusion (spec :
`O:/Users/.../Desktop/spec-fusion-navbtn-urlbar.md` — bureau). Phase A
(edge reveal, `d35f606`) + fixes (`0856a65`) + Phase B gestes (v1.2.0)
livrées. **2 bugs connus en discovery (NB-D1, NB-D2 — causes identifiées,
fix trivial 2 lignes)** : clic gauche inerte (contrat window.URLBar20 non
exposé) + double son middle. NavBtn original : désactivé dans Sine.
URLBar-2.0 : v1.10.1 (`95819b2`) + v1.10.2 contrat (`5ac99df`) poussés.
Énigme "bouton carré" résolue : artefact de cadrage de capture (le bouton
est une capsule conforme au disque/git depuis le 03/09).

## Journal
- [livré] `ba54fb9` v1.0.0 — clone étalonnage NavBtn (capsule identique)
- [livré] `d35f606` v1.1.0 — Phase A : edge reveal (bord droit 40px, timer 2000ms gelé, anti-flicker)
- [livré] `0856a65` v1.1.1 — fixes : séparateur |, solo mono-tab, reveal toggle
- [livré] v1.2.0 — Phase B : gestes fusion (clic gauche urlbar [NB-D1 inert], middle ctrlTab, droit ping-pong, molette réservée) — 2 bugs → discovery
