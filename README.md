# Trends In AI Federated Learning Spam & Ham

## Project Overzicht
Dit project demonstreert de toepassing van Federated Learning voor spam e-mailclassificatie met behulp van de `spam.csv` dataset. Het belangrijkste doel is het verkennen van het gebruik van federated learning met differentiële privacy, modelprestatie-aggregatie en hyperparameter-tuning.

## Belangrijkste Kenmerken
1. **Simuleren van Klanten**: De dataset wordt verdeeld over meerdere klanten met verschillende niveaus van data-heterogeniteit.
2. **Lokale Modeltraining**: Elke klant traint een logistiek regressiemodel met hyperparameter-tuning via cross-validation en past differentiële privacy toe door Laplace-ruis toe te voegen aan de gewichten.
3. **Federated Averaging**: De modellen worden geaggregeerd met behulp van een gewogen gemiddelde techniek, waarbij klanten met meer data of betere prestaties meer bijdragen aan het uiteindelijke model.
4. **Model Evaluatie**: Het model wordt geëvalueerd met behulp van nauwkeurigheid, precisie, recall en de verwarringsmatrix voor elke ronde van federated learning.

## Vereisten
- Python 3.x
- Bibliotheken:
  - pandas
  - numpy
  - scikit-learn
  - matplotlib

## Hoe te Gebruiken
1. Plaats het bestand `spam.csv` in de projectmap.
2. Voer het meegeleverde Python-script uit.
3. Het script traint de modellen in 10 rondes, aggregeert ze met federated averaging en visualiseert de prestatiemetingen (nauwkeurigheid, precisie, recall).

## Output
Het script zal de evaluatieresultaten (nauwkeurigheid, precisie, recall, verwarringsmatrix) voor elke ronde afdrukken en de prestatiemetingen in de loop van de tijd plotten.

## Credits
- Goudantov Bers, 3ITAI
- Loïc Van Camp, 3ITAI