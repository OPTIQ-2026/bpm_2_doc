# BeamScope

Simulation de la propagation d'un faisceau laser gaussien par la méthode
split-step Fourier, avec une interface NiceGUI.

## Milieux étudiés

| Milieu | Phénomène |
|---|---|
| Milieu homogène | Diffraction |
| Guide isolé | Propagation monomode et multimode |
| Coupleur droit | Couplage évanescent |
| Coupleur en S | Passage d'une zone non couplée à une zone couplée |

## Lancer le projet

```bash
python -m venv .venv
.venv\Scripts\activate
python -m pip install -r requirements.txt
python main.py
```

Ouvrir ensuite <http://127.0.0.1:8081>.

Sous macOS ou Linux, activer l'environnement avec `source .venv/bin/activate`.

## Lancer les tests

```bash
python -m unittest discover -s tests -v
```

## Organisation du code

| Fichier | Rôle |
|---|---|
| `propagation.py` | Moteur physique : géométrie, indice, propagation split-step Fourier, modes |
| `analyse.py` | Mesures, fractions de puissance et comptage des modes |
| `graphiques.py` | Carte d'intensité et courbes |
| `export_excel.py` | Export des résultats au format Excel |
| `main.py` | Interface NiceGUI |
| `style.css` | Apparence de l'interface |
| `tests/test_regression.py` | Tests physiques et numériques |

La page [API](api.md) détaille les classes et fonctions.

## Équipe

| Membre | Contribution |
|---|---|
| Shaden Jaziri | À compléter |
| Agathe Abikzer | À compléter |
| Benjamin Angeli | À compléter |