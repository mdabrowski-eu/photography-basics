---
title: "Dlaczego światło liczy się w przysłonach (f-stops)"
weight: 70
---


Zrozumienie systemu wartości przysłony (f-stopów) oraz ich związku z czasem naświetlania i czułością ISO jest fundamentalne dla świadomego kontrolowania ekspozycji w fotografii. System ten, choć na pierwszy rzut oka może wydawać się nieintuicyjny, opiera się na solidnych podstawach fizycznych i matematycznych, które zapewniają jego uniwersalność i precyzję.

### Definicja liczby f (f-stop)

Wartość przysłony, powszechnie określana jako liczba f lub f-stop, jest kluczowym parametrem opisującym, jak dużo światła przepuszcza obiektyw.

**Stosunek ogniskowej obiektywu (f) do średnicy czynnej otworu przysłony (D):** Liczba f (oznaczana jako N) jest definiowana jako stosunek ogniskowej obiektywu (f) do efektywnej średnicy otworu przysłony (D). Matematycznie wyraża się to wzorem: N=f/D Z tego wzoru wynika, że średnica otworu przysłony D=f/N.  

**Dlaczego mniejsza liczba f oznacza większy otwór i więcej światła:** Ponieważ liczba f (N) znajduje się w mianowniku wyrażenia na średnicę (lub średnica D jest w mianowniku wzoru N \= f/D), mniejsza wartość liczbowa N (np. f/1.4, f/2) oznacza większą efektywną średnicę otworu przysłony D. Większa średnica otworu to z kolei większa jego powierzchnia, przez którą może wpadać światło do wnętrza aparatu. Można to przyrównać do ułamków: 1/2 jest wartością większą niż 1/16, stąd przysłona f/2 wpuszcza więcej światła niż f/16.

### Skala wartości f-stop i jej związek z ilością światła

Standardowy szereg wartości przysłony został tak skonstruowany, aby każda kolejna pełna wartość (stopień) zmieniała ilość przepuszczanego światła dokładnie dwukrotnie.

**Standardowy szereg f-stopów:** Typowe pełne stopnie przysłony, które można znaleźć na obiektywach lub w ustawieniach aparatu, to: f/1, f/1.4, f/2, f/2.8, f/4, f/5.6, f/8, f/11, f/16, f/22, f/32, itd.. Współczesne aparaty cyfrowe pozwalają na bardziej precyzyjną regulację przysłony, zazwyczaj w krokach co 1/2 lub 1/3 stopnia EV (wartości ekspozycji).

### **Jak zmiana przysłony wpływa na ilość światła? Wyjaśnienie**

Kluczem do zrozumienia, dlaczego każdy kolejny stopień przysłony (f-stop) zmienia ilość światła dwukrotnie, jest zrozumienie zależności między trzema elementami: **powierzchnią otworu**, jego **średnicą** oraz **liczbą f**.

#### **Krok 1: Liczy się powierzchnia, nie średnica**

Ilość światła, która wpada do aparatu, jest wprost proporcjonalna do **powierzchni** otworu przysłony. Otwór ten jest kołem, a pole powierzchni koła (A) obliczamy ze wzoru, używając jego średnicy (D):

`A = π * (D/2)² = (π * D²) / 4`

Aby **podwoić** ilość wpadającego światła, musimy **podwoić powierzchnię** otworu (A₂ = 2 * A₁). Zobaczmy, jak zmiana ta wpływa na wymaganą średnicę (D):

`(π * D₂²) / 4 = 2 * (π * D₁²) / 4`

Po uproszczeniu wzoru przez usunięcie z obu stron `π` oraz `/4` otrzymujemy:

`D₂² = 2 * D₁²`

A po wyciągnięciu pierwiastka z obu stron:

`D₂ = D₁ * √2`

**Wniosek:** Aby **podwoić powierzchnię** otworu (i wpuścić dwa razy więcej światła), jego **średnica** musi wzrosnąć o czynnik **√2** (czyli około 1,41).

---

#### **Krok 2: Czym jest liczba f (f-number)?**

Liczba f (oznaczana jako N) to stosunek ogniskowej obiektywu (f) do średnicy otworu przysłony (D):

`N = ogniskowa (f) / średnica (D)`

Z tego wzoru wynika, że liczba f jest **odwrotnie proporcjonalna** do średnicy otworu.
* **Większa średnica** (więcej światła) = **mniejsza liczba f** (np. f/1.4).
* **Mniejsza średnica** (mniej światła) = **większa liczba f** (np. f/16).

---

#### **Krok 3: Łączymy wszystko w całość**

Skoro wiemy już wszystko, połączmy te fakty:

* **Aby zmniejszyć ilość światła o połowę** (czyli zamknąć przysłonę o 1 stopień, np. z f/2.8 na f/4), musimy zmniejszyć **powierzchnię** dwukrotnie. Wymaga to zmniejszenia **średnicy** o czynnik √2. Aby to osiągnąć, **liczba f musi zostać pomnożona przez √2**.
  * *Przykład:* `f/2.8 * √2 ≈ f/4`

* **Aby zwiększyć ilość światła dwukrotnie** (czyli otworzyć przysłonę o 1 stopień, np. z f/4 na f/2.8), musimy zwiększyć **powierzchnię** dwukrotnie. Wymaga to zwiększenia **średnicy** o czynnik √2. Aby to osiągnąć, **liczba f musi zostać podzielona przez √2**.
  * *Przykład:* `f/4 / √2 ≈ f/2.8`

#### **Standardowy szereg wartości przysłony**

Dlatego właśnie standardowy szereg wartości przysłony jest tworzony przez kolejne mnożenie (lub dzielenie) przez pierwiastek z dwóch (≈ 1.4).

**f/1, f/1.4, f/2, f/2.8, f/4, f/5.6, f/8, f/11, f/16, f/22**

Każdy kolejny krok w prawo w tym szeregu oznacza **zmniejszenie ilości światła o połowę**. Każdy krok w lewo oznacza jej **podwojenie**.

### Wartość Ekspozycji (EV – Exposure Value)

Wartość Ekspozycji (EV) to ustandaryzowana skala używana w fotografii do określenia ilości światła.

* **Definicja EV:** EV jest skalą logarytmiczną o podstawie 2\. Służy do opisania kombinacji ustawień czasu naświetlania i wartości przysłony, które dają ten sam poziom naświetlenia matrycy, lub do określenia luminancji (jasności) fotografowanej sceny. W praktyce, światłomierz aparatu często wskazuje odchyłkę od "poprawnej" ekspozycji w jednostkach EV; zdjęcie idealnie naświetlone według wskazań światłomierza ma umownie 0 EV.  
* **Jak zmiana o 1 EV odpowiada dwukrotnej zmianie ilości światła:** Zmiana ekspozycji o \+1 EV oznacza dwukrotne zwiększenie ilości światła docierającego do matrycy (np. zdjęcie staje się jaśniejsze). Zmiana o \-1 EV oznacza dwukrotne zmniejszenie ilości światła (zdjęcie staje się ciemniejsze). Każda zmiana wartości przysłony o jeden pełny stopień, czasu naświetlania o jeden pełny stopień (np. z 1/125 s na 1/250 s lub odwrotnie) lub czułości ISO o jeden pełny stopień (np. z ISO 100 na ISO 200 lub odwrotnie) odpowiada zmianie ekspozycji o 1 EV.

### Trójkąt ekspozycji

Ekspozycja zdjęcia, czyli całkowita ilość światła zarejestrowana przez matrycę, jest determinowana przez trzy wzajemnie powiązane parametry: wartość przysłony (f-stop), czas naświetlania (długość otwarcia migawki) oraz czułość ISO matrycy.1 Te trzy elementy tworzą tzw. "trójkąt ekspozycji".

* **Wzajemne zależności między przysłoną, czasem naświetlania i czułością ISO:** Aby uzyskać prawidłowo naświetlone zdjęcie (czyli dostarczyć do matrycy odpowiednią ilość światła), fotograf musi zbalansować te trzy ustawienia. Zmiana jednego z nich wpływa na wymaganą wartość pozostałych.  
* **Jak zmiana jednego parametru o określoną liczbę stopni EV musi być skompensowana zmianą innego parametru, aby utrzymać ten sam poziom ekspozycji:** Kluczową zasadą jest to, że aby zachować ten sam całkowity poziom naświetlenia (to samo EV), zwiększenie ilości światła przez jeden parametr (np. otwarcie przysłony o 1 EV) musi być skompensowane zmniejszeniem ilości światła przez inny parametr o tę samą wartość EV (np. skrócenie czasu naświetlania o 1 EV lub zmniejszenie ISO o 1 EV).  
  * Na przykład, jeśli przymkniemy przysłonę o jeden stopień (np. z f/2.8 na f/4), co zmniejsza ilość światła o połowę (-1 EV), musimy, aby zachować tę samą ekspozycję:  
    * albo dwukrotnie wydłużyć czas naświetlania (np. z 1/500 s na 1/250 s, co daje \+1 EV),  
    * albo dwukrotnie zwiększyć czułość ISO (np. z ISO 100 na ISO 200, co daje \+1 EV),  
    * albo zastosować kombinację zmian czasu i ISO, która sumarycznie da \+1 EV.  
* **Praktyczne przykłady przeliczeń:** 44  
  * Załóżmy, że prawidłowa ekspozycja dla danej sceny to ISO 200, f/8, 1/125 s.  
  * Jeśli chcemy uzyskać mniejszą głębię ostrości i otwieramy przysłonę do f/4 (co oznacza \+2 EV, bo f/8 \-\> f/5.6 \-\> f/4), musimy zmniejszyć ilość światła o 2 EV za pomocą czasu i/lub ISO. Możemy np. skrócić czas do 1/500 s (1/125s \-\> 1/250s \-\> 1/500s, czyli \-2 EV), pozostawiając ISO 200\. Nowe ustawienia to ISO 200, f/4, 1/500 s.  
  * Jeśli chcemy zamrozić bardzo szybki ruch i potrzebujemy czasu 1/1000 s (z 1/125 s to zmiana o \-3 EV, bo 1/125s \-\> 1/250s \-\> 1/500s \-\> 1/1000s), a przysłona f/8 ma pozostać bez zmian, musimy zwiększyć ISO o 3 EV (ISO 200 \-\> 400 \-\> 800 \-\> 1600). Nowe ustawienia to ISO 1600, f/8, 1/1000 s.

Poniższa tabela ilustruje przykłady ekwiwalentnych ekspozycji, dających ten sam poziom naświetlenia (to samo EV), ale różne efekty wizualne:

| Cel / Efekt Artystyczny | ISO | Przysłona (f-stop) | Czas naświetlania (s) | Przybliżone EV |
| :---- | :---- | :---- | :---- | :---- |
| Standardowa ekspozycja (przykład) | 200 | f/8 | 1/125 | \~13 |
| **Mniejsza głębia ostrości** | 200 | **f/4** | **1/500** | \~13 |
| (otwarcie przysłony o 2 EV, |  | (+2 EV) | (-2 EV) |  |
| skrócenie czasu o 2 EV) |  |  |  |  |
| **Większa głębia ostrości** | 200 | **f/16** | **1/30** | \~13 |
| (przymknięcie przysłony o 2 EV, |  | (-2 EV) | (+2 EV) |  |
| wydłużenie czasu o 2 EV) |  |  |  |  |
| **Zamrożenie ruchu** | **800** | f/8 | **1/500** | \~13 |
| (skrócenie czasu o 2 EV, | (+2 EV) |  | (-2 EV) |  |
| zwiększenie ISO o 2 EV) |  |  |  |  |
| **Rozmycie ruchu (np. woda)** | **100** | **f/22** | **1/4** | \~13 |
| (zmniejszenie ISO o 1 EV, | (-1 EV) | (-3 EV) | (+4 EV) |  |
| przymknięcie przysłony o 3 EV, |  |  |  |  |
| znaczne wydłużenie czasu o 4 EV) |  |  |  |  |

Standaryzacja systemu f-stopów, oparta na czynniku 2​, jest niezwykle istotna, ponieważ tworzy uniwersalny język opisu ekspozycji, niezależny od konkretnego obiektywu, jego fizycznej wielkości czy ogniskowej. F-stop normalizuje średnicę otworu względem ogniskowej, a użycie skali opartej na 2​ gwarantuje, że zmiana o jeden pełny stopień f zawsze oznacza dwukrotną zmianę ilości światła. Dzięki temu fotograf może przewidywalnie kontrolować ekspozycję, nawet zmieniając obiektywy – f/2.8 na jednym obiektywie wpuszcza tyle samo światła co f/2.8 na innym (pomijając niewielkie różnice w transmisji światła przez soczewki, które opisuje bardziej precyzyjna, ale rzadziej stosowana skala T-stop). Ta standaryzacja jest fundamentem wymienności obiektywów i umożliwia stosowanie uniwersalnych zasad ekspozycji oraz zewnętrznych światłomierzy.

Co więcej, logarytmiczna natura skali EV (i powiązanych z nią skal przysłony, czasu i ISO) dobrze koresponduje ze sposobem, w jaki ludzkie oko postrzega zmiany jasności. Ludzka percepcja jasności nie jest liniowa; abyśmy postrzegali równomierne przyrosty jasności, fizyczna ilość światła musi rosnąć geometrycznie (co opisuje prawo Webera-Fechnera w psychofizyce). Skala EV, gdzie każdy stopień oznacza podwojenie ilości światła, jest więc bardziej intuicyjna dla fotografa i upraszcza myślenie o ekspozycji. Zamiast operować na bezwzględnych wartościach luminancji, fotografowie mogą myśleć w kategoriach "stopni" lub "działek" ekspozycji, co ułatwia szybkie i precyzyjne dostosowywanie ustawień.

