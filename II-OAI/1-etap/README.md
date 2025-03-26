# Zadania
Na początku nazwy pliku znajduje się liczba punktów na testowym zbiorze (nie walidacyjnym)

# Sposoby rozwiązywania

## Monety
- Różnego rodzaju augmentacje (rotacja, color jitter, odbicie, etc.)
- Circle Hought Transform - [100_monety_d.ipynb](1.monety/100_monety_d.ipynb)
- Podział na różne etapy (detekcja tła, klasyfikacja monet, regresja bounding boxów) - [64_monety_b.ipynb](1.monety/64_monety_b.ipynb)
- Segmentacja tło/moneta, detekcja monet (BFS), klasyfikacja monet - [72_monety_a.ipynb](1.monety/72_monety_a.ipynb)
- FasterRCNN - [78_monety_g.ipynb](1.monety/78_monety_g.ipynb), [94_monety_f.ipynb](1.monety/94_monety_f.ipynb), [95_monety_j.ipynb](1.monety/95_monety_j.ipynb), [100_monety_e.ipynb](1.monety/100_monety_e.ipynb)
- ssd300_vgg16 - [80_monety_c.ipynb](1.monety/80_monety_c.ipynb)

## Halucynacje
- Cechy: dane statyczne prawdopodobieństw (skew, kurtosis, median, kwantyl, max, min, entropy, std, etc.), dane statyczne overlapingu odpowiedzi (między main-supporting, supporting-supporting, po tokenach, bigram, słownie, etc.), długość odpowiedzi, dane statyczne na temat liczb, tfidf vectorize (cosine similarity, pca) (i wiele więcej w poszczególnych rozwiązaniach)
- XGBClassifier - [68_halucynacje_f.ipynb](2.halucynacje/68_halucynacje_f.ipynb), [76_halucynacje_b.ipynb](2.halucynacje/76_halucynacje_b.ipynb), [76_halucynacje_c.ipynb](2.halucynacje/76_halucynacje_c.ipynb), [81_halucynacje_a.ipynb](2.halucynacje/81_halucynacje_a.ipynb), [95_halucynacje_e.ipynb](2.halucynacje/95_halucynacje_e.ipynb), [100_halucynacje_p.ipynb](2.halucynacje/100_halucynacje_p.ipynb)
- models ensemble (XGBClassifier, RandomForestClassifier, LogisticRegression, etc.) - [73_halucynacje_k.ipynb](2.halucynacje/73_halucynacje_k.ipynb), [90_halucynacje_g.ipynb](2.halucynacje/90_halucynacje_g.ipynb) (2 xgboost classifiers), 

## EKG
- Cechy: max, min sygnału, średnia fft sygnału, wartości statystyczne pochodnej sygnału, konkretne indeksy (w odległości od maximum/minimum) sygnału po konwolucji, płaskość piku, energia fali, wysokośc pików po lewej i prawej stronie zespołu QRS, itp. 
- Detekcja PQRS i liczenie cech w oparciu o to - [ekg/100_ekg_e.ipynb](3.ekg/100_ekg_e.ipynb)

## Szum
- Samplowanie części batcha/balansowanie danych + sortowanie po lossie - [100_szum_b.ipynb](4.szum/100_szum_b.ipynb), [100_szum_c.ipynb](4.szum/100_szum_c.ipynb), [100_szum_e.ipynb](4.szum/100_szum_e.ipynb), [100_szum_f.ipynb](4.szum/100_szum_f.ipynb) (quantile, not sort), [100_szum_k.ipynb](4.szum/100_szum_k.ipynb), [100_szum_n.ipynb](4.szum/100_szum_n.ipynb), [100_szum_o.ipynb](4.szum/100_szum_o.ipynb)
- [JoCoR](https://arxiv.org/pdf/2003.02752) - [100_szum_g.ipynb](4.szum/100_szum_g.ipynb)

## Podciągi
Ponieważ zbiór W miał moc 3 można było robić regresje lub klasyfikacje (8 elementów).
- GRU + warstwy/a liniowe/a - [88_podciagi_k.ipynb](5.podciagi//88_podciagi_k.ipynb), [99_podciagi_a.ipynb](5.podciagi//99_podciagi_a.ipynb), [100_podciagi_f.ipynb](5.podciagi//100_podciagi_f.ipynb)
- Conv + MLP - [81_podciagi_c.ipynb](5.podciagi//81_podciagi_c.ipynb), [82_podciagi_b.ipynb](5.podciagi//82_podciagi_b.ipynb)
- LSTM - [97_podciagi_g.ipynb](5.podciagi//97_podciagi_g.ipynb), [99_podciagi_i.ipynb](5.podciagi//99_podciagi_i.ipynb)
- GRU + Attention - [100_podciagi_e.ipynb](5.podciagi//100_podciagi_e.ipynb)
