# Notatniki edukacyjne Neuronovo

Materiały koła naukowego Neuronovo przy Politechnice Wrocławskiej. Objaśnienia i komentarze w kodzie są po polsku. Korzystamy z bezpłatnych danych, modeli i narzędzi.

## PolEmo2: rozpoznawanie wydźwięku tekstów

Porównujemy siedem metod: przewidywanie najczęstszej klasy, TF-IDF z naiwnym klasyfikatorem Bayesa, dwa warianty TF-IDF z regresją logistyczną, średnią polskich wektorów fastText z regresją logistyczną, zamrożony polski enkoder z regresją logistyczną oraz dostrajanie enkodera.

Badamy dwa osobne protokoły: oficjalny podział `all_text` i uczenie na `hotels_text/train`, wybór parametrów na `hotels_text/validation`, a następnie ocenę na `medicine_text/test`. Najlepsze parametry i checkpoint wybiera wyłącznie walidacja.

- [1. Python i pierwsze klasyfikatory — zacznij tutaj](https://colab.research.google.com/github/Neuronovo/notebooks/blob/main/polemo2/01-klasyfikacja-tekstu.ipynb)
- [2. Polski model językowy](https://colab.research.google.com/github/Neuronovo/notebooks/blob/main/polemo2/02-maly-encoder.ipynb)
- [Cały materiał w jednym notatniku](https://colab.research.google.com/github/Neuronovo/notebooks/blob/main/polemo2/00-pelne-porownanie.ipynb)
- [Opis zadania, metod i rzeczywiste wyniki](https://neuronovo.si/projekty/polemo2/)

Materiał uwzględnia osoby z pierwszego semestru studiów. Pierwsza część wyjaśnia zmienne, listy, słowniki, pętle i funkcje. Następnie pokazuje liczenie słów, TF-IDF oraz dwa klasyfikatory na wymyślonych tekstach. Dalej znajdziesz objaśnienia metryk, podziału danych i kolejnych metod. Druga część wprowadza tokenizację, reprezentacje tekstu i uczenie wag sieci. Pytania i ćwiczenia pomagają sprawdzić zrozumienie kodu.

Kliknij odnośnik Colaba, zaloguj się na własne konto Google i wybierz **Plik → Zapisz kopię na Dysku**. Następnie wykonuj komórki od góry. Jedna końcowa komórka uruchamia oba doświadczenia; w drugim modele uczą się od początku na tekstach hotelowych. Dla dostrajania wybierz bezpłatne GPU T4, jeżeli jest dostępne. Dostępność GPU i długość sesji zależą od bieżących limitów Colaba; materiały nie wymagają abonamentu.

Każdy notatnik jest samodzielny: wyjaśnienia przeplatają się z kodem. Nie trzeba przesyłać dodatkowego modułu Pythona ani używać klucza API. Dane i wagi modeli są pobierane bezpośrednio z publicznych źródeł. Nie przechowujemy ich w tym repozytorium.

Kod ćwiczeń: MIT. Dane i gotowe modele mają odrębne licencje podane w notatnikach.
