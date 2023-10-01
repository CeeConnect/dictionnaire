# Dictionnaire CEE

Ce projet propose un vocabulaire uniformisé de référence au format YAML pour les acteurs du dispositif des Certificats d'Economies d'Energie (CEE), permettant la description, la validation et le partage de ressources.

## Structure du dictionnaire

**enums**: Regroupe les termes définis par un ensemble fermé de valeurs (eg une zone climatique n'accepte que trois constantes : H1, H2 et H3). Les énumérations peuvent être également sous-divisées par secteur d'application, un même terme pouvant avoir une définition différente selon le contexte.

**formats**: Regroupe les termes dont les valeurs doivent respecter une nomenclature (eg un numéro SIREN est une chaîne de neuf caractères numériques).

**mixins**: Regroupe les termes composés (eg une adresse est composée d'un numéro, d'une voie, d'un code postal...)

**bundles**: Regroupe les ressources (eg un dépôt, un contrôle, une opération...)

## Usages

- Validation de données JSON (JSON Schema)
- Description APIs (OpenAPI)

## Spécification

- [JSON Schema](https://json-schema.org/) 2020-12

## Roadmap

Couverture par secteur d'application :

- [] Agriculture
- [x] Bâtiment résidentiel
- [] Bâtiment tertiaire
- [] Industrie
- [] Réseau
- [] Transport
