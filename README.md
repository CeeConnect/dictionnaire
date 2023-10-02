# Dictionnaire CEE

Ce projet propose un vocabulaire uniformisé de référence au format YAML pour les acteurs du dispositif des Certificats d'Economies d'Energie (CEE), permettant la description, la validation et le partage de ressources.

## Structure du dictionnaire

**enums**: Regroupe les termes définis par un ensemble fermé de valeurs (eg une zone climatique n'accepte que trois constantes : H1, H2 et H3). Les énumérations peuvent être également sous-divisées par secteur d'application, un même terme pouvant avoir une définition différente selon le contexte.

**formats**: Regroupe les termes dont les valeurs doivent respecter une nomenclature (eg un numéro SIREN est une chaîne de neuf caractères numériques).

**mixins**: Regroupe les termes composés (eg une adresse est composée d'un numéro, d'une voie, d'un code postal...)

**bundles**: Regroupe les ressources métiers (eg un dépôt, un contrôle, une opération...)

## Usages

- Validation de données JSON (JSON Schema)
- Description APIs (OpenAPI)

## Spécification

- [JSON Schema](https://json-schema.org/) 2020-12

## Releases

### v1.0.0

- Couverture des dépôts
- Couverture du secteur résidentiel

### @next

- BAR-SE-109v54-1
- BAR-TH-123v54-2
- BAR-TH-127v54-5
- BAR-TH-160v54-4
- BAR-TH-161v54-2
- BAR-TH-170v54-1

### @beta-v2.0.0

- Couverture des contrôles sur le secteur résidentiel

### @alpha-v3.0.0

- Couverture des dépôts et contrôles de tous les secteurs d'application

## Roadmap

Couverture par secteur d'application :

- [] Agriculture
- [x] Bâtiment résidentiel
- [] Bâtiment tertiaire
- [] Industrie
- [] Réseau
- [] Transport

## Doctrines

### Performances des équipements

Les performances et caractéristiques des équipements mentionnées par les fiches d'opérations standardisées couvertent par une réglementation nationale ou européenne ne sont pas validées. Elles sont considérées de facto cohérente avec le cadre réglementaire.

###  BAR-EN-108v37-2

**L'attesation sur l'honneur prévoit la possibilité de renseigner plusieurs marques et référence dans le cas d'équipements installés de caractéristiques différentes, mais un unique champs relatif à la résistance thermique additionnelle.**

Afin de simplifier le dispositif, il est retenu qu'une fiche d'opération standardisée ne s'applique qu'à un ensemble cohérent d'équipements éligibles. Ainsi il conviendra de réaliser n dossiers avec n partie A de l'attestation sur l'honneur pour n équipements de caractéristiques différentes.
