# Zadania
Na początku nazwy pliku znajduje się liczba punktów na testowym zbiorze (nie walidacyjnym)

# Sposoby rozwiązywania

## Monety
- Różnego rodzaju augmentacje (rotacja, color jitter, odbicie, etc.)
- Circle Hought Transform - [100_monety_d.ipynb](1.monety/100_monety_d.ipynb)
- Podział na różne etapy (detekcja tła, klasyfikacja monet, regresja bounding boxów) - [064_monety_b.ipynb](1.monety/064_monety_b.ipynb)
- Segmentacja tło/moneta, detekcja monet (BFS), klasyfikacja monet - [072_monety_a.ipynb](1.monety/072_monety_a.ipynb)
- FasterRCNN - [078_monety_g.ipynb](1.monety/078_monety_g.ipynb), [094_monety_f.ipynb](1.monety/094_monety_f.ipynb), [095_monety_j.ipynb](1.monety/095_monety_j.ipynb), [100_monety_e.ipynb](1.monety/100_monety_e.ipynb)
- ssd300_vgg16 - [080_monety_c.ipynb](1.monety/080_monety_c.ipynb)

## Halucynacje
- Cechy: dane statyczne prawdopodobieństw (skew, kurtosis, median, kwantyl, max, min, entropy, std, etc.), dane statyczne overlapingu odpowiedzi (między main-supporting, supporting-supporting, po tokenach, bigram, słownie, etc.), długość odpowiedzi, dane statyczne na temat liczb, tfidf vectorize (cosine similarity, pca) (i wiele więcej w poszczególnych rozwiązaniach)
- XGBClassifier - [068_halucynacje_f.ipynb](2.halucynacje/068_halucynacje_f.ipynb), [076_halucynacje_b.ipynb](2.halucynacje/076_halucynacje_b.ipynb), [076_halucynacje_c.ipynb](2.halucynacje/076_halucynacje_c.ipynb), [081_halucynacje_a.ipynb](2.halucynacje/081_halucynacje_a.ipynb), [095_halucynacje_e.ipynb](2.halucynacje/095_halucynacje_e.ipynb), [100_halucynacje_p.ipynb](2.halucynacje/100_halucynacje_p.ipynb)
- models ensemble (XGBClassifier, RandomForestClassifier, LogisticRegression, etc.) - [073_halucynacje_k.ipynb](2.halucynacje/073_halucynacje_k.ipynb), [090_halucynacje_g.ipynb](2.halucynacje/090_halucynacje_g.ipynb) (2 xgboost classifiers), 

## EKG
- Cechy: max, min sygnału, średnia fft sygnału, wartości statystyczne pochodnej sygnału, konkretne indeksy (w odległości od maximum/minimum) sygnału po konwolucji, płaskość piku, energia fali, wysokośc pików po lewej i prawej stronie zespołu QRS, itp. 
- Detekcja PQRS i liczenie cech w oparciu o to - [ekg/100_ekg_e.ipynb](3.ekg/100_ekg_e.ipynb)

## Szum
- Samplowanie części batcha/balansowanie danych + sortowanie po lossie - [100_szum_b.ipynb](4.szum/100_szum_b.ipynb), [100_szum_c.ipynb](4.szum/100_szum_c.ipynb), [100_szum_e.ipynb](4.szum/100_szum_e.ipynb), [100_szum_f.ipynb](4.szum/100_szum_f.ipynb) (quantile, not sort), [100_szum_k.ipynb](4.szum/100_szum_k.ipynb), [100_szum_n.ipynb](4.szum/100_szum_n.ipynb), [100_szum_o.ipynb](4.szum/100_szum_o.ipynb)
- [JoCoR](https://arxiv.org/pdf/2003.02752) - [100_szum_g.ipynb](4.szum/100_szum_g.ipynb)

## Podciągi
Ponieważ zbiór W miał moc 3 można było robić regresje lub klasyfikacje (8 elementów).
- GRU + warstwy/a liniowe/a - [088_podciagi_k.ipynb](5.podciagi/088_podciagi_k.ipynb), [099_podciagi_a.ipynb](5.podciagi/099_podciagi_a.ipynb), [100_podciagi_f.ipynb](5.podciagi//100_podciagi_f.ipynb)
- Conv + MLP - [081_podciagi_c.ipynb](5.podciagi/081_podciagi_c.ipynb), [082_podciagi_b.ipynb](5.podciagi/082_podciagi_b.ipynb)
- LSTM - [097_podciagi_g.ipynb](5.podciagi/097_podciagi_g.ipynb), [099_podciagi_i.ipynb](5.podciagi/099_podciagi_i.ipynb)
- GRU + Attention - [100_podciagi_e.ipynb](5.podciagi/100_podciagi_e.ipynb)
