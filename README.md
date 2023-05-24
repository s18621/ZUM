# ZUM NLP Projekt

Projekt został stworzony w zeszytach Jupiter w Google Colab. Aby uruchomić projekt od początku, należy wykonywać wszystkie klasy po kolej, począwszy od `Setup`. Najlpiej również usunąć wszystkie instejące pliki `.csv`, a także wszystkie modele `.model` wygenerowane przez program.

## Table of Contents
- [Setup](#setup)
- [Gather Data from Tweets](#gather_data_from_tweets)
- [Clean data and remove stopwords](#clean_data_and_remove_stopwords)
- [Create word embeddings](#create_word_embeddings)
- [Modele](#modele)

## Setup

W sekcji setup, do środowiska zostają pobrane wszystkie niezbędne importy w dalszych sekcjach, a także zostają poprane innfe funkcjonalności.

## Gather Data from Tweets

W tej sekcji pobierane są dane tweetów poprzez webscraping `tweepy`. Tweety dotyczą wydarzenia z obecnego miesiąca, to znaczy z Eurowizji 2023. Dane zbierane są z miesiąca. Obecnie w projekcie już znajdują się pliki `.csv` tego powodu możliwe jest pominięcie tego etapu, należy jedynie umieścić te pliki w ścierzce domyślniej MyDrive. 
**Jeżeli pomijamy etap pobiernia i czyszczenia, konieczne jest jednak uruchomienie pierwszego bloku kodu z etapu [Create word embeddings]. [**

## Clean data and remove stopwords

W tym etapie dane są czyszczone. Zostają usunięte wszelkie linki, znaki specjalnie, hashtagi czy odwołania `@`. Usunięte zostają również stop wyrazy aby usprwnić prace w późniejszych etapach.

## Create word embeddings

Na tym etapie zostaje stworzona reprezentacja wektorowa pobranych wcześniej tweetów. Do tego dzielone są na dwie klasy poprzez `KMeans`

## Modele

Po uruchomieniu wszystkich poprzednich kroków, możliwe jest następnie uruchomienie zakładek `Neural Model`, `Classic ML`, oraz `Language Model`. Wszystkie te modele zapiszą do plików pliki w formacie `.model`. Aby przyspieszyć ich działanie, preferowane jest włączenie środowiska Colab wykorzystujące GPU. Obecnie w projekcie już znajdują się pliki `.model` z tego powodu możliwe jest pominięcie etapu uczenia sieci neuronowej. 

# Kontakt
W razie pytań proszę o kontakt na platformie teams lub przez maila uczelnianego.
