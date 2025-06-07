---
title: "4.2 Matryca jako materiał światłoczuły – rodzaje i jak działa"
weight: 5
---


### **Wprowadzenie do matrycy: serce aparatu cyfrowego**

Matryca światłoczuła jest fundamentalnym komponentem każdego aparatu cyfrowego, pełniącym rolę analogiczną do błony filmowej w fotografii tradycyjnej. Jej zadaniem jest przechwytywanie światła wpadającego przez obiektyw i przekształcanie go na sygnał elektryczny.1 Ten sygnał jest następnie przetwarzany przez procesor obrazu w celu stworzenia finalnego zdjęcia cyfrowego.1 Zrozumienie zasady działania matrycy jest kluczowe dla pojęcia całego procesu fotograficznego w erze cyfrowej.

Każda matryca zbudowana jest z milionów miniaturowych elementów światłoczułych, nazywanych pikselami.1 Każdy z tych pikseli działa jak mały detektor, rejestrujący intensywność światła, które na niego pada w danym momencie ekspozycji. To właśnie z informacji zebranych przez poszczególne piksele odtwarzany jest cały obraz.4

### **Fizyka działania fotodiody w pikselu**

Sercem każdego piksela, zarówno w matrycach typu CCD, jak i CMOS, jest fotodioda. Jest to element półprzewodnikowy, którego podstawową funkcją jest konwersja energii świetlnej (fotonów) na ładunek elektryczny (elektrony).

#### **Struktura P-N i polaryzacja wsteczna**

Fotodiody są zazwyczaj strukturami półprzewodnikowymi typu P-N, co oznacza, że składają się z dwóch warstw materiału półprzewodnikowego (najczęściej krzemu) o różnym typie domieszkowania: typu P (z nadmiarem dziur, czyli dodatnich nośników ładunku) i typu N (z nadmiarem elektronów, czyli ujemnych nośników ładunku).6 Na granicy tych dwóch warstw tworzy się tzw. złącze P-N, a wokół niego powstaje obszar zubożony (ang. *depletion region*), pozbawiony swobodnych nośników ładunku.8

W matrycach światłoczułych fotodiody pracują zazwyczaj w trybie polaryzacji wstecznej (ang. *reverse bias*).6 Oznacza to, że do warstwy typu P przykładany jest potencjał ujemny, a do warstwy typu N potencjał dodatni. Taka polaryzacja prowadzi do poszerzenia obszaru zubożonego, co ma kluczowe znaczenie dla efektywności detekcji światła. Szerszy obszar zubożony zwiększa prawdopodobieństwo, że padający foton zostanie zaabsorbowany właśnie w tym obszarze, gdzie wygenerowane nośniki ładunku mogą być efektywnie rozdzielone i zebrane. Ponadto, polaryzacja wsteczna zmniejsza pojemność złącza, co przekłada się na szybszą odpowiedź fotodiody na zmiany oświetlenia.8

#### **Proces konwersji fotonów na elektrony (generowanie par elektron-dziura)**

Gdy foton o energii równej lub większej niż szerokość przerwy energetycznej materiału półprzewodnikowego (dla krzemu jest to około 1.12 eV, co odpowiada światłu widzialnemu i bliskiej podczerwieni) pada na fotodiodę, może zostać zaabsorbowany.9 Absorpcja fotonu skutkuje wybiciem elektronu z pasma walencyjnego do pasma przewodnictwa. W miejscu, z którego elektron został wybity, powstaje "dziura" o ładunku dodatnim. W ten sposób tworzona jest para elektron-dziura.6 Ten proces, znany jako wewnętrzny efekt fotoelektryczny, jest podstawą działania fotodiody.12 Istotne jest, że liczba wygenerowanych par elektron-dziura jest wprost proporcjonalna do liczby padających fotonów, a więc do natężenia światła.12

#### **Gromadzenie ładunku w studni potencjału, separacja nośników przez pole elektryczne**

W obszarze zubożonym, poszerzonym przez polaryzację wsteczną, istnieje silne wewnętrzne pole elektryczne. To pole odgrywa kluczową rolę w separacji nowo powstałych par elektron-dziura.8 Elektrony (o ładunku ujemnym) są przyciągane w kierunku dodatnio naładowanej warstwy N, natomiast dziury (o ładunku dodatnim) przemieszczają się w kierunku ujemnie naładowanej warstwy P.9

Elektrony, które są nośnikami sygnału w większości matryc, są następnie gromadzone w specjalnie ukształtowanym obszarze pod elektrodą piksela, zwanym "studnią potencjału" (ang. *potential well*).4 Pojemność tej studni, określana jako *Full Well Capacity* (FWC), definiuje maksymalną liczbę elektronów, jaką dany piksel może zgromadzić przed osiągnięciem stanu nasycenia.16 Im więcej fotonów padnie na piksel, tym więcej elektronów zgromadzi się w studni potencjału, aż do jej całkowitego wypełnienia.

#### **Prąd ciemny i jego wpływ**

Nawet w całkowitej ciemności, bez padającego światła, w materiale półprzewodnikowym zachodzą procesy termicznego generowania par elektron-dziura. Prowadzi to do powstawania niewielkiego prądu, zwanego prądem ciemnym (ang. *dark current*).7 Prąd ciemny jest niepożądanym zjawiskiem, ponieważ dodaje szum do sygnału użytecznego (pochodzącego od światła) i może ograniczać zdolność detekcji bardzo słabych sygnałów.8 Poziom prądu ciemnego jest silnie zależny od temperatury matrycy – rośnie wykładniczo wraz ze wzrostem temperatury – oraz od czasu ekspozycji.17 Z tego powodu w zaawansowanych zastosowaniach, np. w astrofotografii, matryce są często chłodzone, aby zminimalizować prąd ciemny i poprawić stosunek sygnału do szumu.3

### **Rodzaje matryc światłoczułych**

Na rynku dominują dwa główne typy matryc światłoczułych: CCD (Charge-Coupled Device) oraz CMOS (Complementary Metal-Oxide-Semiconductor). Chociaż podstawowy mechanizm konwersji światła na ładunek w pikselu jest w obu przypadkach podobny (oparty na fotodiodzie), różnią się one znacząco architekturą, sposobem odczytu sygnału oraz charakterystyką działania.

#### **CCD (Charge-Coupled Device)**

Matryce CCD były historycznie pierwszym szeroko stosowanym typem sensorów w aparatach cyfrowych i przez długi czas uznawane były za oferujące wyższą jakość obrazu.13

* **Architektura piksela i zasada działania:** W matrycy CCD ładunek (elektrony) zgromadzony w każdym pikselu podczas ekspozycji jest transferowany sekwencyjnie, niczym woda w wiadrach przekazywanych z rąk do rąk. Ładunki z poszczególnych pikseli w rzędzie są przesuwane do rejestru odczytu, a następnie ładunki z tego rejestru są kolejno transferowane do jednego, wspólnego dla całej matrycy (lub jej części) wzmacniacza i przetwornika analogowo-cyfrowego (ADC).2 Ten proces powtarzany jest dla każdego rzędu pikseli.2  
* **Zalety:** Matryce CCD charakteryzowały się tradycyjnie bardzo dobrą jakością obrazu, niskim poziomem szumów (szczególnie szumu stałowzorcowego, dzięki scentralizowanemu wzmacnianiu), wysoką czułością oraz dużym współczynnikiem wypełnienia piksela (ang. *fill factor*), co oznacza, że większa część powierzchni piksela była aktywna światłoczułe.13 Naturalną cechą matryc CCD jest również tzw. migawka globalna (ang. *global shutter*), gdzie wszystkie piksele rozpoczynają i kończą ekspozycję jednocześnie, co jest korzystne przy fotografowaniu szybko poruszających się obiektów.12  
* **Wady:** Głównymi wadami matryc CCD są: stosunkowo wolny odczyt danych (konieczność sekwencyjnego transferu ładunków), wyższe zużycie energii w porównaniu do CMOS oraz bardziej skomplikowany i droższy proces produkcji.13 Są również podatne na zjawisko zwane "bloomingiem", czyli przelewaniem się nadmiaru ładunku z nasyconego piksela do sąsiednich, co objawia się jako pionowe smugi na obrazie w miejscu silnych prześwietleń.23

#### **CMOS (Complementary Metal-Oxide-Semiconductor)**

Matryce CMOS, początkowo stosowane w mniej wymagających aplikacjach, dzięki intensywnemu rozwojowi technologicznemu zdominowały rynek aparatów cyfrowych, od smartfonów po profesjonalne aparaty pełnoklatkowe.2

* **Architektura piksela (Active Pixel Sensor \- APS):** Kluczową różnicą w matrycach CMOS jest to, że każdy piksel (lub mała grupa pikseli) posiada własną, zintegrowaną elektronikę, w tym wzmacniacz sygnału, a często także elementy przetwornika analogowo-cyfrowego.13 Taka architektura nazywana jest Aktywnym Pikselem Sensorycznym (APS).15 Ładunek zgromadzony w fotodiodzie jest konwertowany na napięcie bezpośrednio w obrębie piksela, a następnie to napięcie jest odczytywane indywidualnie dla każdego piksela poprzez adresowanie, podobnie jak w pamięciach komputerowych.2  
* **Zalety:** Matryce CMOS oferują znacznie szybszy odczyt danych niż CCD, co umożliwia realizację takich funkcji jak szybkie zdjęcia seryjne, nagrywanie wideo w wysokiej rozdzielczości i z dużą liczbą klatek na sekundę, a także selektywny odczyt fragmentów obrazu ("okienkowanie").13 Charakteryzują się również znacznie niższym zużyciem energii oraz niższym kosztem produkcji, ponieważ mogą być wytwarzane w standardowych procesach technologicznych używanych do produkcji innych układów scalonych CMOS (np. procesorów, pamięci).12 Pozwalają także na większą integrację dodatkowych funkcji (np. przetwarzania obrazu, redukcji szumów) bezpośrednio na chipie matrycy.2  
* **Wady:** Wczesne generacje matryc CMOS cierpiały na wyższy poziom szumów w porównaniu do CCD, szczególnie szumu stałowzorcowego (FPN), wynikającego z niejednorodności wzmacniaczy w poszczególnych pikselach.2 Miały również niższą czułość i mniejszy współczynnik wypełnienia piksela, ponieważ część jego powierzchni zajmowała elektronika.21 Większość matryc CMOS wykorzystuje tzw. migawkę kroczącą (ang. *rolling shutter*), gdzie kolejne linie pikseli są odczytywane sekwencyjnie, co może prowadzić do zniekształceń obrazu szybko poruszających się obiektów (efekt "galaretki").2 Dostępne są jednak również matryce CMOS z migawką globalną, eliminujące ten problem.  
* **Nowoczesne technologie CMOS:**  
  * **BSI (Back-Side Illumination):** Technologia "oświetlenia od tyłu" polega na odwróceniu tradycyjnej struktury piksela CMOS. Warstwa z połączeniami metalicznymi i tranzystorami jest przenoszona pod warstwę światłoczułą (krzemową). Dzięki temu światło padające na matrycę ma bezpośredni dostęp do fotodiod, nie będąc blokowane ani rozpraszane przez elementy elektroniki. Skutkuje to znacznym wzrostem współczynnika wypełnienia i efektywności zbierania światła, co przekłada się na wyższą czułość i lepszą jakość obrazu, szczególnie w przypadku pikseli o małych rozmiarach.2  
  * **Stacked CMOS (Matryce warstwowe):** W tej zaawansowanej technologii warstwa pikseli jest oddzielona od warstwy obwodów przetwarzających sygnał i ułożona nad nią. Obie warstwy są ze sobą połączone. Pozwala to na jeszcze większą integrację zaawansowanych funkcji przetwarzania obrazu bezpośrednio na chipie matrycy oraz na bardzo szybki odczyt danych, co jest kluczowe np. dla wideo w ultra wysokiej rozdzielczości i z ekstremalnie dużą liczbą klatek na sekundę.

Ewolucja technologii CMOS, napędzana potrzebą miniaturyzacji, szybkości i niższych kosztów, doprowadziła do przezwyciężenia wielu początkowych wad. Presja rynkowa faworyzowała rozwój CMOS, a technologie takie jak BSI stanowiły przełom, rozwiązując problem niskiego współczynnika wypełnienia i czułości. W rezultacie, nowoczesne matryce CMOS oferują jakość obrazu porównywalną, a w niektórych aspektach nawet przewyższającą matryce CCD, przy jednoczesnym zachowaniu swoich inherentnych zalet, takich jak szybkość i niskie zużycie energii. Zrozumienie tej ewolucji jest kluczowe dla docenienia obecnego stanu technologii sensorów i kierunków jej dalszego rozwoju.

Poniższa tabela podsumowuje kluczowe cechy matryc CCD i CMOS:

| Cecha | CCD (Tradycyjna) | CMOS (Wczesna) | CMOS (Nowoczesna BSI/Stacked) |
| :---- | :---- | :---- | :---- |
| **Jakość obrazu (ogólnie)** | Bardzo dobra, niska szumowość | Zwykle niższa, wyższe szumy FPN | Bardzo dobra, porównywalna lub lepsza od CCD |
| **Czułość** | Wysoka | Niższa | Wysoka, szczególnie BSI |
| **Współczynnik wypełnienia** | Wysoki | Niższy (elektronika w pikselu) | Wysoki (dzięki BSI) |
| **Szumy (ogólnie)** | Niskie, zwłaszcza FPN | Wyższe, zwłaszcza FPN | Niskie, zaawansowana redukcja FPN |
| **Szybkość odczytu** | Wolna (sekwencyjny transfer) | Szybsza (adresowalny odczyt) | Bardzo szybka (równoległy odczyt, stacked) |
| **Zużycie energii** | Wysokie | Niskie | Bardzo niskie |
| **Koszt produkcji** | Wyższy (specjalistyczny proces) | Niższy (standardowy proces CMOS) | Niższy/umiarkowany |
| **Migawka (typowo)** | Globalna | Krocząca (Rolling shutter) | Krocząca lub Globalna |
| **Integracja funkcji** | Ograniczona | Możliwa (np. ADC na chipie) | Wysoka (zaawansowane przetwarzanie na chipie) |
| **Blooming** | Podatna | Mniej podatna | Dobrze kontrolowany |

### **Charakterystyka popularnych formatów matryc**

Rozmiar fizyczny matrycy światłoczułej ma fundamentalny wpływ na wiele aspektów jakości obrazu i charakterystyki aparatu. Do najpopularniejszych formatów należą \[12 (link zewn. fotoblogia.pl)\]:

* **Pełna klatka (Full Frame, ok. 36x24 mm):** Ten format odpowiada rozmiarowi pojedynczej klatki tradycyjnego filmu małoobrazkowego (35 mm). Matryce pełnoklatkowe, dzięki swojej dużej powierzchni, oferują zazwyczaj najlepszą jakość obrazu, charakteryzującą się niskim poziomem szumów (szczególnie przy wysokich czułościach ISO), szerokim zakresem dynamicznym oraz możliwością łatwego uzyskania małej głębi ostrości, co jest pożądane np. w fotografii portretowej. Są one standardem w profesjonalnych i zaawansowanych amatorskich aparatach cyfrowych (lustrzankach i bezlusterkowcach).  
* **APS-C (Advanced Photo System type-C):** Matryce APS-C są mniejsze od pełnoklatkowych, a ich dokładne wymiary mogą się nieznacznie różnić w zależności od producenta (np. ok. 23.6x15.6 mm dla Nikon/Sony/Fuji lub 22.2x14.8 mm dla Canon). Stanowią one popularny wybór w lustrzankach i bezlusterkowcach skierowanych do entuzjastów fotografii, oferując dobry kompromis między jakością obrazu, rozmiarem aparatu i obiektywów oraz ceną systemu.  
* **Mikro Cztery Trzecie (Micro Four Thirds \- MFT, ok. 17.3x13 mm):** Ten format jest jeszcze mniejszy od APS-C i został opracowany wspólnie przez firmy Olympus (obecnie OM System) i Panasonic dla ich systemów aparatów bezlusterkowych. Mniejszy rozmiar matrycy MFT pozwala na konstruowanie bardziej kompaktowych aparatów i obiektywów, co jest zaletą dla osób ceniących mobilność.

Wpływ rozmiaru matrycy na kąt widzenia (współczynnik kadrowania \- crop factor):  
Mniejsze matryce, w porównaniu do matrycy pełnoklatkowej, "widzą" węższy fragment obrazu rzutowanego przez ten sam obiektyw. Zjawisko to opisuje tzw. współczynnik kadrowania (ang. crop factor). Jest to liczba, przez którą należy pomnożyć nominalną ogniskową obiektywu, aby uzyskać ogniskową dającą taki sam kąt widzenia na matrycy pełnoklatkowej. Na przykład, dla matryc APS-C współczynnik kadrowania wynosi typowo ok. 1.5x (Nikon, Sony, Fuji) lub 1.6x (Canon), a dla systemu Mikro Cztery Trzecie ok. 2x. Oznacza to, że obiektyw o ogniskowej 50 mm założony na aparat z matrycą APS-C (crop 1.5x) da kąt widzenia odpowiadający obiektywowi 75 mm na pełnej klatce.  
Wpływ rozmiaru matrycy na głębię ostrości:  
Rozmiar matrycy ma również istotny wpływ na głębię ostrości. Przy tej samej wartości liczbowej przysłony (np. f/2.8) i tym samym kącie widzenia (co oznacza użycie obiektywu o krótszej rzeczywistej ogniskowej na mniejszej matrycy, aby uzyskać ten sam kadr co na matrycy pełnoklatkowej), mniejsze matryce dają większą głębię ostrości.27 Jest to złożone zjawisko, wynikające z faktu, że dla uzyskania tego samego kadru na mniejszej matrycy używamy obiektywu o krótszej ogniskowej, co samo w sobie prowadzi do większej głębi ostrości. Dodatkowo, aby uzyskać obraz o tej samej wielkości z mniejszej matrycy, wymagane jest większe powiększenie, co wpływa na postrzegany rozmiar krążka rozproszenia i tym samym na akceptowalną głębię ostrości. Zrozumienie tej zależności jest kluczowe, gdy celem jest świadome manipulowanie głębią ostrości, np. w celu uzyskania silnego rozmycia tła.  
Poniższa tabela zestawia charakterystykę popularnych formatów matryc:

| Cecha | Pełna klatka (Full Frame) | APS-C | Mikro Cztery Trzecie (MFT) |
| :---- | :---- | :---- | :---- |
| **Przybliżone wymiary (mm)** | 36 x 24 | np. 23.6 x 15.6 lub 22.2 x 14.8 | 17.3 x 13 |
| **Współczynnik kadrowania** | 1x (referencyjny) | ok. 1.5x \- 1.6x | ok. 2x |
| **Typowe zalety** | Najlepsza jakość obrazu, niskie szumy, duży DR, mała głębia ostrości (łatwość uzyskania) | Dobry kompromis: jakość/rozmiar/cena, duży wybór systemów | Kompaktowy rozmiar systemu, dobra jakość obrazu |
| **Typowe wady** | Duży rozmiar i waga systemu, wysoka cena | Większa głębia ostrości niż FF (przy tym samym kadrze i f-stop), nieco wyższe szumy niż FF | Mniejsza matryca \= potencjalnie wyższe szumy i mniejszy DR niż większe formaty, większa głębia ostrości |
| **Przykładowe zastosowania** | Fotografia profesjonalna, portretowa, krajobrazowa, sportowa, studyjna | Fotografia zaawansowana, hobbystyczna, podróżnicza, codzienna | Fotografia podróżnicza, uliczna, filmowanie, systemy wymagające kompaktowości |

### **Wpływ wielkości piksela i gęstości pikseli na jakość obrazu**

Parametry takie jak fizyczny rozmiar pojedynczego piksela oraz całkowita liczba pikseli na matrycy (gęstość pikseli) mają bezpośredni i złożony wpływ na kluczowe aspekty jakości obrazu, w tym czułość, poziom szumów, zakres dynamiczny oraz postrzeganą rozdzielczość.29

#### **Czułość (ISO) i współczynnik wypełnienia (fill factor)**

Większe piksele, ze względu na swoją większą powierzchnię, są w stanie zebrać więcej fotonów w danym czasie ekspozycji. Prowadzi to do silniejszego sygnału elektrycznego, co generalnie przekłada się na lepszy stosunek sygnału do szumu (SNR) i wyższą rzeczywistą czułość matrycy.17 Oznacza to, że przy słabym oświetleniu matryce z większymi pikselami mogą produkować obrazy o lepszej jakości z mniejszą ilością szumów przy tej samej wartości ISO.

Współczynnik wypełnienia (ang. *fill factor*) to parametr określający, jaka część całkowitej powierzchni piksela jest faktycznie światłoczuła.26 Im wyższy współczynnik wypełnienia, tym efektywniej piksel zbiera światło. W tradycyjnych matrycach CMOS (szczególnie typu FSI \- Front-Side Illumination), część powierzchni piksela zajmowana jest przez tranzystory i metalowe ścieżki, co zmniejsza współczynnik wypełnienia.4 Problem ten jest częściowo rozwiązywany przez stosowanie mikrosoczewek nad każdym pikselem, które skupiają światło na obszarze światłoczułym.2 Jeszcze lepsze rezultaty daje wspomniana wcześniej technologia BSI, gdzie warstwa światłoczuła znajduje się nad elektroniką, maksymalizując efektywną powierzchnię zbierającą światło.2

#### **Poziom szumów**

Szum jest nieodłącznym elementem obrazu cyfrowego i pochodzi z różnych źródeł. Jego poziom i charakter zależą od wielu czynników, w tym od wielkości pikseli.

* **Szum śrutowy (Photon Shot Noise):** Ten rodzaj szumu wynika bezpośrednio z kwantowej natury światła. Liczba fotonów docierających do danego piksela w określonym czasie podlega naturalnym fluktuacjom statystycznym (opisywanym przez rozkład Poissona).33 Szum śrutowy jest proporcjonalny do pierwiastka kwadratowego z natężenia sygnału (liczby zebranych fotonów) i jest najbardziej widoczny w jaśniejszych partiach obrazu.34 Większe piksele, zbierając więcej fotonów, generują silniejszy sygnał, co może prowadzić do lepszego stosunku sygnału do szumu śrutowego.  
* **Szum termiczny (Dark Current Noise):** Jak wspomniano wcześniej, jest on wynikiem termicznego generowania elektronów w krzemie, nawet przy braku światła.33 Jego poziom rośnie wraz z temperaturą matrycy i czasem naświetlania.17 Chociaż większe piksele mogą mieć mniejszy prąd ciemny na jednostkę powierzchni, całkowity prąd ciemny zależy również od technologii wykonania i temperatury pracy.  
* **Szum odczytu (Read Noise):** Jest to szum wprowadzany przez elektronikę matrycy podczas procesu odczytu ładunku zgromadzonego w pikselach i jego konwersji na sygnał cyfrowy.16 Obejmuje on szum wzmacniaczy, szum kwantyzacji przetwornika A/C oraz, w przypadku matryc CMOS, tzw. szum resetu (kTC noise).34 Szum odczytu jest generalnie niezależny od ilości światła (sygnału) i dominuje w najciemniejszych partiach obrazu.34 Wielkość piksela sama w sobie nie musi bezpośrednio determinować poziomu szumu odczytu, który bardziej zależy od architektury i jakości elektroniki odczytującej.  
* **Szum stałowzorcowy (Fixed Pattern Noise \- FPN):** Wynika z niewielkich, ale stałych różnic w charakterystyce poszczególnych pikseli, takich jak różnice w prądzie ciemnym (DSNU \- Dark Signal Non-Uniformity) lub różnice w odpowiedzi na światło (PRNU \- Photo Response Non-Uniformity).18 FPN był większym problemem we wczesnych matrycach CMOS, ale nowoczesne techniki kalibracji i korekcji wbudowane w aparaty i oprogramowanie znacznie go redukują.18

Większe piksele, dzięki zdolności do zbierania większej ilości fotonów (silniejszy sygnał), często oferują lepszy ogólny stosunek sygnału do szumu, co przekłada się na czystsze obrazy, szczególnie w trudnych warunkach oświetleniowych i przy wyższych czułościach ISO.

#### **Zakres dynamiczny (Dynamic Range \- DR)**

Zakres dynamiczny matrycy określa jej zdolność do jednoczesnego rejestrowania bardzo jasnych i bardzo ciemnych obszarów sceny bez utraty szczegółów (tj. bez prześwietleń w światłach i bez utonięcia w szumach w cieniach).16 Jest on definiowany jako stosunek maksymalnego sygnału, jaki piksel może zarejestrować przed nasyceniem (określonego przez jego pojemność studni potencjału \- FWC), do poziomu szumów w najciemniejszych obszarach (zazwyczaj zdominowanego przez szum odczytu).17

Większe piksele zazwyczaj charakteryzują się większą pojemnością studni potencjału (FWC), ponieważ mają fizycznie więcej miejsca na gromadzenie elektronów.17 Przy podobnym poziomie szumu odczytu, większa FWC bezpośrednio przekłada się na szerszy zakres dynamiczny.17 Dlatego matryce z większymi pikselami (np. pełnoklatkowe o umiarkowanej liczbie megapikseli) często oferują lepszy zakres dynamiczny niż matryce z bardzo małymi, gęsto upakowanymi pikselami.

#### **Pojemność studni potencjału (Full Well Capacity \- FWC)**

FWC to maksymalna liczba elektronów, jaką pojedynczy piksel może zgromadzić i przechować przed osiągnięciem stanu nasycenia.16 Po przekroczeniu FWC, piksel nie jest w stanie zarejestrować więcej światła, a nadmiarowy ładunek może "przelewać się" do sąsiednich pikseli (zjawisko bloomingu, bardziej typowe dla CCD) lub po prostu prowadzić do utraty informacji w prześwietlonych obszarach.23 FWC jest bezpośrednio związana z fizycznym rozmiarem fotodiody w pikselu – większa fotodioda generalnie oznacza większą FWC.17 Większa FWC jest pożądana, ponieważ przyczynia się do wyższego stosunku sygnału do szumu w jasnych partiach obrazu i szerszego zakresu dynamicznego.

#### **Rozdzielczość a percepcja szczegółów**

Większa liczba pikseli na matrycy (czyli wyższa gęstość pikseli) teoretycznie oznacza wyższą rozdzielczość, czyli zdolność do odwzorowania drobniejszych detali sceny.29 Jednakże, jeśli duża liczba pikseli jest upakowana na małej matrycy, poszczególne piksele stają się bardzo małe. Jak omówiono powyżej, bardzo małe piksele mogą cierpieć z powodu wyższego poziomu szumów, mniejszej czułości i węższego zakresu dynamicznego. W rezultacie, chociaż teoretyczna rozdzielczość może być wysoka, rzeczywista zdolność do rozróżniania drobnych szczegółów, zwłaszcza w trudnych warunkach oświetleniowych lub przy dużym kontraście sceny, może być ograniczona przez szumy i inne niedoskonałości sygnału. Istnieje zatem pewien kompromis między dążeniem do jak największej liczby megapikseli a utrzymaniem wysokiej "jakości" sygnału z każdego piksela. To wyjaśnia, dlaczego profesjonalne aparaty często stawiają na optymalny balans między rozdzielczością a wielkością piksela, zamiast na samą maksymalizację liczby megapikseli.

Związek między fizycznym rozmiarem piksela a "jakością" sygnału jest fundamentalny. Większe piksele generalnie oferują lepszy stosunek sygnału do szumu (SNR), większy zakres dynamiczny (DR) i wyższą czułość. Wynika to z faktu, że większy piksel ma większą powierzchnię zbierającą fotony, co prowadzi do silniejszego sygnału dla danego poziomu oświetlenia. Ponadto, większy piksel często oznacza większą pojemność studni potencjału (FWC), co pozwala na zgromadzenie większej liczby elektronów przed nasyceniem. Przy założeniu, że poziom szumu odczytu jest w dużej mierze niezależny od rozmiaru piksela, a szum śrutowy jest zależny od sygnału, silniejszy sygnał i większa FWC prowadzą do lepszego SNR i DR. Dlatego, przy tej samej generacji technologii, matryce z większymi pikselami (np. pełnoklatkowe o umiarkowanej liczbie megapikseli) często lepiej radzą sobie w słabym świetle i oferują szerszy zakres tonalny. Wybór aparatu z określoną wielkością matrycy i liczbą pikseli to zatem kompromis. Więcej megapikseli na małej matrycy oznacza mniejsze piksele, co może negatywnie wpłynąć na jakość obrazu w trudnych warunkach, mimo wyższej teoretycznej rozdzielczości.

Warto również zwrócić uwagę na percepcję "crop factora" i jego wpływu na głębię ostrości. Współczynnik kadrowania wynika z mniejszego rozmiaru matrycy, która "wycina" fragment obrazu rzutowanego przez obiektyw. Aby uzyskać ten sam kadr (to samo pole widzenia) na matrycy z crop factorem, trzeba użyć obiektywu o krótszej ogniskowej. Głębia ostrości zależy od przysłony, odległości od obiektu i rzeczywistej ogniskowej. Przy tej samej liczbie f i tym samym kadrze, mniejsza matryca da większą głębię ostrości. Dzieje się tak, ponieważ krótsza ogniskowa sama w sobie daje większą DOF. Aby uzyskać tę samą głębię ostrości co na pełnej klatce, na mniejszej matrycy trzeba by użyć proporcjonalnie szerszego otworu przysłony. Zrozumienie tego niuansu jest kluczowe dla świadomego wyboru sprzętu i technik fotografowania, szczególnie gdy celem jest specyficzna kontrola nad głębią ostrości.

