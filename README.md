# spectropy

Outils Python pour l'analyse et la visualisation de spectres astronomiques d'amateur.

Ce dépôt rassemble une collection de notebooks Colab/Jupyter développés pour le
traitement de spectres acquis avec un spectrographe **Alpy 600** (et calibrés sous
**ISIS**), ainsi que divers outils de préparation d'observations et de comparaison
avec des données professionnelles. Les notebooks sont majoritairement en français,
pensés pour être exécutés dans Google Colab.

## Contenu

### Visualisation et analyse de spectres

- **Spectre_2D_nebuleuses.ipynb** — Représentation 2D (longueur d'onde × position
  sur la fente) de spectres de nébuleuses, à partir d'un FITS issu d'ISIS.
  Prétraitement de l'histogramme (normalisation + étirement asinh), colorisation
  physique λ→RGB et annotation des raies d'émission.
- **Analyse_du_spectre_de_NGC4565.ipynb** — Analyse détaillée du spectre de la
  galaxie NGC 4565 (Dn4000, largeurs équivalentes, corrélation croisée, correction
  héliocentrique, courbe de rotation).
- **Visualisation_spectre_Mira.ipynb** — Visualisation annotée de spectres
  d'étoiles variables de type Mira.
- **nova_2026rdg_Halpha.ipynb** — Analyse de la région Hα du spectre de la nova
  AT 2026rdg (Nova Aql 2026).
- **visualisation_spectre_T_CrB.ipynb** — Visualisation du spectre de T CrB.
- **OuvertureSpectreSDSS.ipynb** — Ouverture et exploration de spectres SDSS.

### Spectres de référence et bibliothèques spectrales

- **spectre_atome_v6.ipynb** — Visualisation de spectres atomiques.
- **tableau_periodique_spectres_v3.ipynb** — Spectres associés aux éléments du
  tableau périodique.
- **melchiors_catalog_search.ipynb** — Recherche dans le catalogue MELCHIORS.
- **melchiors_catalog_download_spectrum.ipynb** — Téléchargement de spectres du
  catalogue MELCHIORS.
- **catalogue_Melchiors_AB.ods** — Catalogue MELCHIORS (feuille de calcul).

### Préparation d'observations

- **selection_cibles_etoiles_spectro_Simbad.ipynb** — Sélection de cibles
  stellaires spectroscopiques via SIMBAD (requêtes TAP/ADQL, filtrage par type
  spectral).
- **aavso_variable_star_v5_robuste.ipynb** — Interrogation AAVSO/VizieR pour
  étoiles variables.
- **carte_illumination_satellites.ipynb** — Carte géométrique d'illumination des
  satellites (contamination des poses).

### Outils divers

- **ccf_multi_galaxies.ipynb** — Vitesses radiales par corrélation croisée (CCF)
  sur plusieurs galaxies.
- **calculateur_cosmologique_ned_wright.ipynb** — Calculateur cosmologique
  (portage Python 3 du CC.py de Ned Wright, avec explications pédagogiques).
- **wavelength_tables_crop.csv** — Table de longueurs d'onde de référence.

## Matériel

Spectres acquis avec : télescope Newton 200 mm / C11 SCT, spectrographe Alpy 600,
caméra Atik 414EX, montures ZWO AM5 et AZ-EQ6. Acquisition sous Linux (CCDciel/INDI),
calibration sous ISIS.

## Dépendances

Principalement `numpy`, `matplotlib`, `scipy`, `astropy`, `pandas`. Chaque notebook
installe ses dépendances spécifiques dans sa première cellule (`!pip install ...`).

## Licence

Distribué sous licence MIT. Voir le fichier [LICENSE](LICENSE).
