# **Dogłębne Podstawy Fotografii dla Dociekliwych**

## **4.2 Matryca jako materiał światłoczuły – rodzaje i jak działa**

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

## **5\. Przysłona – jak działa, jak wpływa na obraz, bokeh i głębia ostrości**

Przysłona jest jednym z kluczowych elementów układu optycznego aparatu fotograficznego, pełniącym rolę analogiczną do źrenicy w ludzkim oku.39 Jej głównym zadaniem jest regulacja ilości światła przechodzącego przez obiektyw i docierającego do matrycy światłoczułej, ale ma ona również fundamentalny wpływ na inne aspekty obrazu, takie jak głębia ostrości i charakter rozmycia tła (bokeh).

### **Mechanizm przysłony irysowej**

Większość obiektywów fotograficznych wyposażona jest w tzw. przysłonę irysową.

* **Budowa:** Przysłona irysowa składa się z zestawu cienkich, zachodzących na siebie metalowych blaszek, nazywanych listkami lub lamelami.39 Te listki ułożone są w okrąg i mogą się poruszać, zmieniając średnicę centralnego otworu, przez który przechodzi światło.40  
* **Kształt i liczba listków:** Liczba listków (np. od 5 do 11 lub więcej) oraz ich kształt (proste krawędzie lub zaokrąglone) mają istotny wpływ na wygląd nieostrych punktów światła w tle, czyli efekt bokeh.27 Obiektywy z większą liczbą listków i/lub listkami o zaokrąglonych krawędziach tworzą bardziej okrągły otwór, co przekłada się na gładsze i przyjemniejsze dla oka rozmycie oraz bardziej okrągłe bliki świetlne.27  
* **Sposób regulacji średnicy otworu:** Średnica otworu przysłony jest precyzyjnie kontrolowana przez mechanizm wewnątrz obiektywu. W starszych konstrukcjach regulacja odbywała się manualnie za pomocą pierścienia na obiektywie. W nowoczesnych aparatach odbywa się to najczęściej elektronicznie, poprzez sygnały sterujące wysyłane z korpusu aparatu, które poruszają listkami przysłony do żądanej pozycji.

### **Wpływ otworu przysłony na obraz**

Zmiana wielkości otworu przysłony ma dwojaki, fundamentalny wpływ na finalny obraz: reguluje ilość światła docierającego do matrycy oraz modyfikuje głębię ostrości.

#### **Regulacja ilości światła docierającego do matrycy**

Jest to podstawowa i najbardziej intuicyjna funkcja przysłony. Zgodnie z zasadą działania, większy otwór przysłony (odpowiadający mniejszej wartości liczbowej f, np. f/1.4, f/2) przepuszcza więcej światła do wnętrza aparatu w jednostce czasu.42 Z kolei mniejszy otwór przysłony (odpowiadający większej wartości liczbowej f, np. f/16, f/22) ogranicza ilość przepuszczanego światła.44 Przysłona, obok czasu naświetlania i czułości ISO, stanowi jeden z trzech filarów tzw. trójkąta ekspozycji, pozwalając fotografowi na precyzyjne kontrolowanie jasności zdjęcia.1

#### **Głębia ostrości (DOF – Depth of Field)**

Głębia ostrości to jeden z najważniejszych kreatywnych narzędzi w fotografii, a jej kontrola jest nierozerwalnie związana z ustawieniem przysłony.40

* **Definicja i percepcja ostrości:** Głębia ostrości (DOF) definiowana jest jako zakres odległości, mierzony wzdłuż osi optycznej obiektywu, w którym obiekty na zdjęciu wydają się być "akceptowalnie ostre" dla ludzkiego oka.47 Należy podkreślić, że idealnie ostry jest tylko jeden plan – ten, na który dokładnie ustawiono ostrość. Obiekty znajdujące się bliżej lub dalej od tego planu są w rzeczywistości w pewnym stopniu rozmyte. Głębia ostrości opisuje więc strefę, w której to rozmycie jest na tyle małe, że nie jest dostrzegane jako nieostrość.28  
* Optyka geometryczna głębi ostrości: krążek rozproszenia (Circle of Confusion – CoC):  
  Aby zrozumieć, dlaczego zmiana przysłony wpływa na głębię ostrości, należy wprowadzić pojęcie krążka rozproszenia (CoC).50  
  * Idealny obiektyw skupia wszystkie promienie światła wychodzące z jednego punktu na obiekcie w jednym punkcie na płaszczyźnie matrycy (lub filmu) – pod warunkiem, że ten punkt obiektu leży w płaszczyźnie ostrości.  
  * Jeśli jednak punkt obiektu znajduje się przed lub za płaszczyzną ostrości, promienie światła po przejściu przez obiektyw nie zbiegną się idealnie w jednym punkcie na matrycy, lecz utworzą na niej niewielką, rozmytą plamkę. Kształt tej plamki jest rzutem kształtu otworu przysłony, a dla uproszczenia przyjmuje się, że jest to koło – stąd nazwa "krążek rozproszenia".51  
  * "Akceptowalna wielkość CoC" to maksymalny rozmiar takiego krążka rozproszenia na powierzchni matrycy, który na finalnym obrazie (np. odbitce oglądanej z typowej odległości) będzie wciąż postrzegany przez ludzkie oko jako ostry punkt, a nie jako rozmyta plamka.28 Wartość ta zależy od wielu czynników, m.in. od rozmiaru matrycy, rozdzielczości, zamierzonego powiększenia obrazu oraz odległości i warunków jego oglądania. Dla matryc pełnoklatkowych (36x24 mm) często przyjmuje się standardową wartość CoC w granicach 0.025 mm do 0.030 mm.51  
* **Wpływ wartości przysłony na rozmiar krążka rozproszenia i głębię ostrości:**  
  * **Duży otwór przysłony (mała liczba f, np. f/1.4, f/2.8):** Gdy przysłona jest szeroko otwarta, promienie światła pochodzące z punktów obiektu znajdujących się poza płaszczyzną ostrości tworzą stosunkowo szeroki stożek, który przecina płaszczyznę matrycy, tworząc na niej duże krążki rozproszenia.48 W rezultacie, tylko obiekty znajdujące się bardzo blisko płaszczyzny ostrości będą odwzorowane jako akceptowalnie ostre (ich CoC będzie mniejszy od limitu). Głębia ostrości jest wówczas mała (płytka).42 Jest to pożądane np. w fotografii portretowej, gdzie chcemy wyizolować ostry obiekt od rozmytego tła.40  
  * **Mały otwór przysłony (duża liczba f, np. f/11, f/16):** Gdy przysłona jest mocno domknięta, stożek promieni światła jest znacznie węższy. Nawet dla punktów obiektu znacznie oddalonych od płaszczyzny ostrości, krążki rozproszenia tworzone na matrycy są małe.48 W efekcie, szeroki zakres odległości (zarówno przed, jak i za płaszczyzną ostrości) będzie odwzorowany z akceptowalną ostrością. Głębia ostrości jest wówczas duża (głęboka).42 Jest to wykorzystywane np. w fotografii krajobrazowej, gdzie dąży się do uzyskania ostrości na wszystkich planach, od pierwszego planu po horyzont.40 Wizualizacje tego zjawiska, często przedstawiane jako diagramy promieni (np. 28), pokazują, jak zmiana średnicy otworu przysłony wpływa na kąt zbieżności stożka promieni, a tym samym na rozmiar krążka rozproszenia dla obiektów nie znajdujących się w płaszczyźnie ostrości.  
* **Wpływ odległości fotografowanego obiektu od aparatu:** Im bliżej znajduje się obiekt, na który ustawiona jest ostrość, tym mniejsza jest głębia ostrości, nawet przy tej samej wartości przysłony i ogniskowej obiektywu.53 Jest to szczególnie widoczne w makrofotografii, gdzie głębia ostrości może wynosić zaledwie ułamki milimetra.54 Wynika to z faktu, że przy małych odległościach ostrzenia, względna różnica odległości do obiektów tła i pierwszego planu staje się bardzo duża, a kąty, pod jakimi promienie z tych obiektów wpadają do obiektywu, są bardziej zróżnicowane, co prowadzi do szybszego wzrostu rozmiaru krążków rozproszenia dla punktów poza płaszczyzną ostrości.  
* **Wpływ odległości obiektu od tła:** Im większa jest odległość między ostro sfotografowanym obiektem a tłem, tym bardziej rozmyte będzie tło, ponieważ znajdzie się ono dalej poza (i tak już płytką, jeśli używamy dużej przysłony i/lub długiej ogniskowej) strefą głębi ostrości.27  
* **Wpływ ogniskowej obiektywu:** Przy tej samej wartości przysłony i tej samej odległości od fotografowanego obiektu, obiektywy o dłuższej ogniskowej generalnie dają mniejszą (płytszą) głębię ostrości.27 Dłuższe ogniskowe powodują większe powiększenie tła, w tym również jego rozmycia. Nawet jeśli geometryczny rozmiar krążków rozproszenia na matrycy byłby podobny, ich większe powiększenie w finalnym obrazie sprawia wrażenie płytszej głębi ostrości.  
* **Rozkład głębi ostrości (zasada 1/3 przed, 2/3 za punktem ostrości):** Głębia ostrości nie rozkłada się symetrycznie wokół płaszczyzny, na którą ustawiono ostrość. Zazwyczaj około jedna trzecia głębi ostrości znajduje się przed płaszczyzną ostrości, a dwie trzecie za nią.54 Ten stosunek nie jest jednak stały i zmienia się w zależności od odległości ostrzenia i ogniskowej obiektywu. Przy bardzo małych odległościach ostrzenia (np. w makrofotografii) rozkład głębi ostrości jest bliższy symetrii 1:1. Natomiast przy ostrzeniu na tzw. odległość hiperfokalną, głębia ostrości rozciąga się od około połowy tej odległości aż do nieskończoności. Zrozumienie tego niesymetrycznego rozkładu jest istotne dla precyzyjnego ustawiania ostrości, np. w fotografii portretowej (gdzie ostrość ustawia się na oczy, licząc, że nos i uszy również znajdą się w strefie akceptowalnej ostrości) lub w fotografii krajobrazowej.  
* **Praktyczne zastosowanie kontroli głębi ostrości:** Możliwość manipulowania głębią ostrości jest jednym z podstawowych narzędzi ekspresji w fotografii. Mała głębia ostrości (uzyskiwana przy dużych otworach przysłony, np. f/1.8, f/2.8) pozwala na wyizolowanie głównego obiektu od tła, skupiając na nim uwagę widza – jest to często stosowane w fotografii portretowej, produktowej czy sportowej.40 Duża głębia ostrości (uzyskiwana przy małych otworach przysłony, np. f/11, f/16) zapewnia ostrość na wielu planach zdjęcia, co jest pożądane w fotografii krajobrazowej, architektury czy dokumentalnej, gdzie ważne jest pokazanie kontekstu i szczegółów otoczenia.47

Głębia ostrości jest zjawiskiem nie tylko geometrycznym, ale również percepcyjnym. Definicja "akceptowalnej ostrości" i dopuszczalnego rozmiaru krążka rozproszenia zależy od warunków oglądania finalnego obrazu, jego wielkości (np. mała odbitka vs duży wydruk wystawowy) oraz indywidualnej percepcji widza.28 Optyka geometryczna dostarcza narzędzi do obliczenia rozmiaru krążków rozproszenia na matrycy, ale to, czy dany krążek zostanie uznany za "ostry punkt" czy "rozmytą plamkę", zależy od tego, jak duży będzie on na finalnym obrazie i z jakiej odległości będzie oglądany. Mniejszy wydruk lub większa odległość oglądania pozwalają na większy akceptowalny CoC na matrycy. Dlatego głębia ostrości nie jest wartością absolutną, lecz zależy od kontekstu użytkowania zdjęcia. Fotografowie muszą brać pod uwagę nie tylko ustawienia aparatu, ale także przeznaczenie zdjęcia, aby świadomie kontrolować głębię ostrości.

### **Efekt bokeh**

Termin "bokeh" pochodzi z języka japońskiego i odnosi się do estetycznej jakości rozmycia nieostrych partii obrazu, a w szczególności sposobu, w jaki odwzorowywane są nieostre punkty światła (tzw. bliki).27 Nie chodzi tu jedynie o stopień rozmycia (który zależy od głębi ostrości), ale o jego charakter – czy jest ono gładkie, "kremowe", czy może "nerwowe", z wyraźnymi krawędziami.

* **Optyczne podstawy powstawania efektu bokeh:**  
  * **Rola kształtu listków przysłony:** Kształt otworu przysłony ma bezpośredni i najbardziej widoczny wpływ na kształt krążków rozproszenia (blików) tworzonych przez nieostre punkty światła.27 Gdy przysłona jest maksymalnie otwarta, otwór jest zazwyczaj zbliżony do koła, a bliki są okrągłe. Po przymknięciu przysłony, otwór przybiera kształt wielokąta utworzonego przez listki przysłony, a bliki odwzorowują ten kształt.27 Obiektywy z większą liczbą listków (np. 9, 11\) i listkami o zaokrąglonych krawędziach są w stanie utrzymać bardziej okrągły kształt otworu nawet po przymknięciu, co prowadzi do powstawania bardziej okrągłych i często uważanych za przyjemniejsze dla oka blików bokeh.40  
  * **Wpływ konstrukcji obiektywu i korekcji aberracji:** Jakość i charakter bokeh zależą również w dużym stopniu od ogólnej konstrukcji optycznej obiektywu, a w szczególności od sposobu skorygowania różnych aberracji optycznych.27 Kluczową rolę odgrywa tu aberracja sferyczna.  
    * **Aberracja sferyczna** polega na tym, że promienie światła przechodzące przez różne strefy soczewki (centralną i brzegowe) nie są skupiane w jednym punkcie. Sposób, w jaki ta aberracja jest skorygowana (lub celowo niedokorygowana), wpływa na rozkład jasności wewnątrz krążka rozproszenia. Na przykład, niedokorygowana aberracja sferyczna może prowadzić do powstawania blików z jaśniejszym środkiem i miękkimi krawędziami (tzw. "gładki" lub "mydlany" bokeh), podczas gdy przekorygowana aberracja sferyczna może skutkować blikami z jasnymi, ostrymi krawędziami i ciemniejszym środkiem (tzw. "nerwowy" bokeh).  
    * Inne aberracje, takie jak koma czy astygmatyzm, również mogą wpływać na kształt blików, szczególnie w brzegowych partiach kadru, prowadząc np. do powstawania blików w kształcie "kocich oczu".  
    * Niektóre historyczne lub specjalistyczne konstrukcje obiektywów, jak np. obiektywy Petzvala, są znane z bardzo charakterystycznego, "wirującego" efektu bokeh (ang. *swirly bokeh*), który jest wynikiem specyficznej kombinacji aberracji.55  
  * **Jak kąt padania promieni światła z nieostrych punktów na matrycę, w zależności od otworu przysłony, tworzy charakterystyczne krążki rozproszenia:** Promienie światła wychodzące z punktu znajdującego się poza głębią ostrości, po przejściu przez otwór przysłony, nie skupiają się w jednym punkcie na płaszczyźnie matrycy, lecz tworzą na niej plamkę świetlną. Kształt tej plamki jest wiernym odwzorowaniem kształtu otworu przysłony. Wielkość tej plamki (czyli stopień rozmycia) zależy od tego, jak bardzo dany punkt jest oddalony od płaszczyzny ostrości, oraz od wielkości otworu przysłony – im większy otwór i im dalej punkt od płaszczyzny ostrości, tym większy krążek rozproszenia.

Bokeh jest często uważany za "charakter" lub "duszę" obiektywu, odzwierciedlający specyficzne wybory projektowe i kompromisy dokonane przez jego konstruktorów. Różne obiektywy, nawet o tej samej ogniskowej i jasności, mogą produkować bokeh o zupełnie innym charakterze. Wynika to z faktu, że idealny obiektyw nie istnieje, a każda konstrukcja optyczna jest wynikiem kompromisów między minimalizacją różnych aberracji, ostrością, kontrastem, a także rozmiarem, wagą i ceną. Wybierając obiektyw, szczególnie do zastosowań portretowych czy artystycznych, warto zwracać uwagę nie tylko na jego parametry techniczne, takie jak ostrość, ale także na charakter generowanego przez niego bokeh, który może znacząco wpłynąć na ostateczną estetykę zdjęć.

## **6\. Dlaczego światło liczy się w przysłonach (f-stops) i w jaki sposób przelicza się f-stopy dla migawki, czułości, przysłony etc.**

Zrozumienie systemu wartości przysłony (f-stopów) oraz ich związku z czasem naświetlania i czułością ISO jest fundamentalne dla świadomego kontrolowania ekspozycji w fotografii. System ten, choć na pierwszy rzut oka może wydawać się nieintuicyjny, opiera się na solidnych podstawach fizycznych i matematycznych, które zapewniają jego uniwersalność i precyzję.

### **Definicja liczby f (f-stop)**

Wartość przysłony, powszechnie określana jako liczba f lub f-stop, jest kluczowym parametrem opisującym, jak dużo światła przepuszcza obiektyw.43

* **Stosunek ogniskowej obiektywu (f) do średnicy czynnej otworu przysłony (D):** Liczba f (oznaczana jako N) jest definiowana jako stosunek ogniskowej obiektywu (f) do efektywnej średnicy otworu przysłony (D).46 Matematycznie wyraża się to wzorem: N=f/D Z tego wzoru wynika, że średnica otworu przysłony D=f/N.  
* **Dlaczego mniejsza liczba f oznacza większy otwór i więcej światła:** Ponieważ liczba f (N) znajduje się w mianowniku wyrażenia na średnicę (lub średnica D jest w mianowniku wzoru N \= f/D), mniejsza wartość liczbowa N (np. f/1.4, f/2) oznacza większą efektywną średnicę otworu przysłony D.42 Większa średnica otworu to z kolei większa jego powierzchnia, przez którą może wpadać światło do wnętrza aparatu.43 Można to przyrównać do ułamków: 1/2 jest wartością większą niż 1/16, stąd przysłona f/2 wpuszcza więcej światła niż f/16.57

### **Skala wartości f-stop i jej związek z ilością światła**

Standardowy szereg wartości przysłony został tak skonstruowany, aby każda kolejna pełna wartość (stopień) zmieniała ilość przepuszczanego światła dokładnie dwukrotnie.46

* **Standardowy szereg f-stopów:** Typowe pełne stopnie przysłony, które można znaleźć na obiektywach lub w ustawieniach aparatu, to: f/1, f/1.4, f/2, f/2.8, f/4, f/5.6, f/8, f/11, f/16, f/22, f/32, itd..41 Współczesne aparaty cyfrowe pozwalają na bardziej precyzyjną regulację przysłony, zazwyczaj w krokach co 1/2 lub 1/3 stopnia EV (wartości ekspozycji).57  
* **Wyjaśnienie, dlaczego każda kolejna pełna wartość f-stop zmienia ilość światła dwukrotnie:** Kluczem do zrozumienia tej zależności jest fakt, że ilość światła wpadającego do aparatu jest proporcjonalna do **powierzchni** otworu przysłony, a nie do jego średnicy. Otwór przysłony jest w przybliżeniu kołem, a powierzchnia koła (A) wyraża się wzorem A=π⋅(D/2)2=(π⋅D2)/4. Aby dwukrotnie zwiększyć lub zmniejszyć ilość przepuszczanego światła, należy odpowiednio dwukrotnie zwiększyć lub zmniejszyć powierzchnię otworu przysłony. Załóżmy, że mamy dwie powierzchnie otworu, A1​ i A2​, takie że A2​=2⋅A1​. Wówczas: (π⋅D22​)/4=2⋅(π⋅D12​)/4 Po uproszczeniu otrzymujemy: D22​=2⋅D12​, co prowadzi do D2​=D1​⋅2​. Oznacza to, że aby zmienić ilość światła dwukrotnie (czyli zmienić powierzchnię otworu dwukrotnie), średnica otworu musi zmienić się o czynnik 2​ (w przybliżeniu 1.414).46 Ponieważ liczba f (N) jest odwrotnie proporcjonalna do średnicy otworu (N=f/D), to aby średnica zmieniła się o czynnik 2​ (lub 1/2​), liczba f musi zmienić się również o czynnik 2​ (lub 1/2​). Dlatego kolejne wartości w standardowym szeregu f-stopów są tworzone poprzez mnożenie (lub dzielenie) poprzedniej wartości przez 2​. Na przykład: 1⋅2​≈1.4 1.4⋅2​≈2 2⋅2​≈2.8 2.8⋅2​≈4 I tak dalej. Zatem zmiana wartości przysłony o jeden pełny stopień (np. z f/2.8 na f/4) oznacza zmianę średnicy otworu o czynnik 2​, co skutkuje dwukrotną zmianą powierzchni otworu, a tym samym dwukrotną zmianą ilości przepuszczanego światła.57

### **Wartość Ekspozycji (EV – Exposure Value)**

Wartość Ekspozycji (EV) to ustandaryzowana skala używana w fotografii do określenia ilości światła.44

* **Definicja EV:** EV jest skalą logarytmiczną o podstawie 2\. Służy do opisania kombinacji ustawień czasu naświetlania i wartości przysłony, które dają ten sam poziom naświetlenia matrycy, lub do określenia luminancji (jasności) fotografowanej sceny.44 W praktyce, światłomierz aparatu często wskazuje odchyłkę od "poprawnej" ekspozycji w jednostkach EV; zdjęcie idealnie naświetlone według wskazań światłomierza ma umownie 0 EV.44  
* **Jak zmiana o 1 EV odpowiada dwukrotnej zmianie ilości światła:** Zmiana ekspozycji o \+1 EV oznacza dwukrotne zwiększenie ilości światła docierającego do matrycy (np. zdjęcie staje się jaśniejsze). Zmiana o \-1 EV oznacza dwukrotne zmniejszenie ilości światła (zdjęcie staje się ciemniejsze).44 Każda zmiana wartości przysłony o jeden pełny stopień, czasu naświetlania o jeden pełny stopień (np. z 1/125 s na 1/250 s lub odwrotnie) lub czułości ISO o jeden pełny stopień (np. z ISO 100 na ISO 200 lub odwrotnie) odpowiada zmianie ekspozycji o 1 EV.

### **Trójkąt ekspozycji**

Ekspozycja zdjęcia, czyli całkowita ilość światła zarejestrowana przez matrycę, jest determinowana przez trzy wzajemnie powiązane parametry: wartość przysłony (f-stop), czas naświetlania (długość otwarcia migawki) oraz czułość ISO matrycy.1 Te trzy elementy tworzą tzw. "trójkąt ekspozycji".

* **Wzajemne zależności między przysłoną, czasem naświetlania i czułością ISO:** Aby uzyskać prawidłowo naświetlone zdjęcie (czyli dostarczyć do matrycy odpowiednią ilość światła), fotograf musi zbalansować te trzy ustawienia. Zmiana jednego z nich wpływa na wymaganą wartość pozostałych.45  
* **Jak zmiana jednego parametru o określoną liczbę stopni EV musi być skompensowana zmianą innego parametru, aby utrzymać ten sam poziom ekspozycji:** Kluczową zasadą jest to, że aby zachować ten sam całkowity poziom naświetlenia (to samo EV), zwiększenie ilości światła przez jeden parametr (np. otwarcie przysłony o 1 EV) musi być skompensowane zmniejszeniem ilości światła przez inny parametr o tę samą wartość EV (np. skrócenie czasu naświetlania o 1 EV lub zmniejszenie ISO o 1 EV).44  
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

Standaryzacja systemu f-stopów, oparta na czynniku 2​, jest niezwykle istotna, ponieważ tworzy uniwersalny język opisu ekspozycji, niezależny od konkretnego obiektywu, jego fizycznej wielkości czy ogniskowej.46 F-stop normalizuje średnicę otworu względem ogniskowej, a użycie skali opartej na 2​ gwarantuje, że zmiana o jeden pełny stopień f zawsze oznacza dwukrotną zmianę ilości światła. Dzięki temu fotograf może przewidywalnie kontrolować ekspozycję, nawet zmieniając obiektywy – f/2.8 na jednym obiektywie wpuszcza tyle samo światła co f/2.8 na innym (pomijając niewielkie różnice w transmisji światła przez soczewki, które opisuje bardziej precyzyjna, ale rzadziej stosowana skala T-stop). Ta standaryzacja jest fundamentem wymienności obiektywów i umożliwia stosowanie uniwersalnych zasad ekspozycji oraz zewnętrznych światłomierzy.

Co więcej, logarytmiczna natura skali EV (i powiązanych z nią skal przysłony, czasu i ISO) dobrze koresponduje ze sposobem, w jaki ludzkie oko postrzega zmiany jasności. Ludzka percepcja jasności nie jest liniowa; abyśmy postrzegali równomierne przyrosty jasności, fizyczna ilość światła musi rosnąć geometrycznie (co opisuje prawo Webera-Fechnera w psychofizyce). Skala EV, gdzie każdy stopień oznacza podwojenie ilości światła, jest więc bardziej intuicyjna dla fotografa i upraszcza myślenie o ekspozycji. Zamiast operować na bezwzględnych wartościach luminancji, fotografowie mogą myśleć w kategoriach "stopni" lub "działek" ekspozycji, co ułatwia szybkie i precyzyjne dostosowywanie ustawień.

## **7\. Z czego wynika winietowanie i jak można mu zapobiec**

Winietowanie jest częstym zjawiskiem w fotografii, objawiającym się jako stopniowy spadek jasności lub nasycenia kolorów na brzegach i w rogach kadru w porównaniu do jego centralnej części.60 Może być ono postrzegane jako wada optyczna obiektywu, ale czasami jest również stosowane jako celowy efekt artystyczny, mający na celu skupienie uwagi widza na środku obrazu.60 Zrozumienie przyczyn różnych typów winietowania jest kluczowe dla jego minimalizacji lub świadomego wykorzystania.

### **Rodzaje winietowania i ich szczegółowe przyczyny**

Wyróżnia się kilka głównych rodzajów winietowania, z których każdy ma inne podłoże fizyczne.60

#### **Winietowanie optyczne (naturalne)**

Ten typ winietowania jest nieodłącznie związany z fizyką przechodzenia światła przez układ optyczny obiektywu i jest szczególnie widoczny w obiektywach szerokokątnych oraz jasnych (o dużym otworze względnym) przy maksymalnie otwartej przysłonie.60

* **Fizyczne przyczyny:**  
  * **Prawo cos⁴θ (spadek natężenia oświetlenia dla promieni skośnych):** Jest to najbardziej fundamentalna przyczyna winietowania naturalnego. Wynika ona z faktu, że promienie światła padające na brzegi matrycy (lub filmu) docierają do niej pod pewnym kątem (θ) względem osi optycznej, w przeciwieństwie do promieni padających na centrum matrycy, które biegną niemal prostopadle. Istnieją trzy główne efekty składające się na to prawo:  
    1. Efektywna powierzchnia zbierająca światło przez piksel na brzegu matrycy jest mniejsza o czynnik cos(θ) w porównaniu do piksela w centrum (dla tej samej wiązki światła).  
    2. Odległość od źrenicy wyjściowej obiektywu do brzegu matrycy jest większa niż do centrum o czynnik 1/cos(θ), co zgodnie z prawem odwrotnych kwadratów dla natężenia światła, zmniejsza natężenie oświetlenia o czynnik cos²(θ).  
    3. Efektywny rozmiar źrenicy wyjściowej obiektywu, widziany z punktu na brzegu matrycy, może być mniejszy o czynnik cos(θ) (tzw. efekt "pupil compression" lub "vignetting by the aperture stop itself"). Połączenie tych efektów prowadzi do spadku natężenia oświetlenia na brzegach matrycy proporcjonalnego do cos⁴(θ).60  
  * **Konstrukcja obiektywu:** Winietowanie optyczne wynika również z samej konstrukcji obiektywu. Soczewki mają ograniczoną średnicę, a promienie światła przechodzące przez ich zewnętrzne części (szczególnie przedniej i tylnej grupy soczewek) mogą być częściowo "przycinane" lub absorbowane przez oprawy poszczególnych soczewek lub przez samą obudowę obiektywu, zanim dotrą do płaszczyzny matrycy.60 Jest to szczególnie problematyczne w przypadku jasnych obiektywów szerokokątnych, gdzie kąty padania światła są duże.  
* **Wpływ otworu przysłony:** Winietowanie optyczne jest zazwyczaj najbardziej widoczne przy maksymalnie otwartej przysłonie. Przymykanie przysłony (zwiększanie liczby f) często znacząco redukuje ten typ winietowania.60 Dzieje się tak, ponieważ mniejszy otwór przysłony ogranicza wiązkę światła do bardziej centralnej części soczewek, gdzie transmisja światła jest bardziej równomierna i mniej podatna na ograniczenia wynikające ze średnicy soczewek.60

Całkowite wyeliminowanie winietowania optycznego w fazie projektowania obiektywu, szczególnie szerokokątnego i jasnego, wymagałoby zastosowania soczewek o bardzo dużej średnicy i skomplikowanej konstrukcji, co prowadziłoby do znacznego wzrostu rozmiaru, wagi i ceny obiektywu. Dlatego konstruktorzy często idą na kompromis, akceptując pewien poziom winietowania, który może być później skorygowany cyfrowo.

#### **Winietowanie mechaniczne**

Ten rodzaj winietowania powstaje, gdy fizyczne elementy, niebędące integralną częścią układu optycznego soczewek, blokują lub przesłaniają drogę światła na brzegach pola widzenia.60

* **Przyczyny:**  
  * **Filtry fotograficzne:** Stosowanie filtrów o zbyt grubych oprawkach, a zwłaszcza nakładanie kilku filtrów jeden na drugi (tzw. "stacking"), może powodować winietowanie mechaniczne, szczególnie w przypadku obiektywów szerokokątnych, gdzie pole widzenia jest bardzo szerokie.60  
  * **Osłony przeciwsłoneczne:** Użycie nieodpowiedniej osłony przeciwsłonecznej (np. przeznaczonej do obiektywu o dłuższej ogniskowej na obiektywie szerokokątnym) lub jej nieprawidłowe zamocowanie (np. przekręcenie osłony tulipanowej) może prowadzić do zasłonięcia rogów kadru.60  
  * **Inne akcesoria:** Winietowanie mechaniczne mogą również powodować inne akcesoria montowane na przedniej części obiektywu, takie jak niektóre adaptery do filtrów, konwertery szerokokątne lub telekonwertery, jeśli ich wewnętrzna średnica jest zbyt mała w stosunku do pola widzenia obiektywu.  
* **Charakterystyka:** Winietowanie mechaniczne często objawia się jako gwałtowne, całkowite zaciemnienie rogów obrazu, czasami z wyraźnie widoczną, ostrą krawędzią przesłaniającego elementu.60 Wpływ przysłony na ten typ winietowania jest zazwyczaj mniejszy niż na winietowanie optyczne; jeśli coś fizycznie blokuje światło, przymknięcie przysłony może jedynie nieco zmienić kształt zaciemnionego obszaru.

#### **Winietowanie pikselowe (związane z sensorem)**

Ten typ winietowania, nazywany również winietowaniem cyfrowym, występuje wyłącznie w aparatach cyfrowych i jest związany z konstrukcją samej matrycy światłoczułej oraz sposobem, w jaki piksele zbierają światło.60

* **Przyczyny:**  
  * **Mikrosoczewki:** Większość współczesnych matryc światłoczułych posiada warstwę mikrosoczewek umieszczonych nad każdym pikselem. Ich zadaniem jest skupienie jak największej ilości światła padającego na powierzchnię piksela na jego światłoczułym obszarze (fotodiodzie), co zwiększa efektywność zbierania światła, zwłaszcza w przypadku małych pikseli. Jednakże, efektywność tych mikrosoczewek może spadać dla promieni światła padających na matrycę pod dużym kątem (co ma miejsce na brzegach i w rogach sensora).  
  * **Kątowa czułość pikseli:** Same fotodiody, będące elementami światłoczułymi, wykazują największą czułość na światło padające prostopadle do ich powierzchni. Promienie światła padające pod znacznym kątem są absorbowane mniej efektywnie, co prowadzi do osłabienia sygnału generowanego przez piksele znajdujące się na brzegach matrycy.60 Ten efekt potęguje naturalne winietowanie optyczne.  
* **Wpływ konstrukcji obiektywu:** Obiektywy o konstrukcji telecentrycznej po stronie obrazu (ang. *image-space telecentric lenses*) są zaprojektowane tak, aby główne promienie świetlne padały na całą powierzchnię matrycy możliwie jak najbardziej prostopadle. Takie obiektywy minimalizują winietowanie pikselowe. Są one częściej spotykane w systemach z mniejszymi matrycami (np. Mikro Cztery Trzecie) oraz w zastosowaniach przemysłowych i naukowych, gdzie równomierność oświetlenia jest krytyczna.60

Warto zauważyć, że obserwowane na zdjęciu winietowanie jest często sumą efektów różnych typów. Na przykład, naturalne winietowanie optyczne może być potęgowane przez winietowanie pikselowe. Jeśli dodatkowo użyjemy nieodpowiedniego filtra, nałoży się na to jeszcze winietowanie mechaniczne. Diagnozując problem, należy rozważyć wszystkie potencjalne przyczyny.

### **Metody zapobiegania i korygowania winietowania**

Istnieje szereg metod pozwalających na minimalizację winietowania na etapie fotografowania oraz na jego korekcję w procesie postprodukcji.60

#### **Na etapie fotografowania**

* **Dobór obiektywu:** Niektóre obiektywy, szczególnie te wyższej klasy, są projektowane z myślą o minimalizacji winietowania. Przed zakupem warto zapoznać się z testami i recenzjami obiektywów, które często zawierają pomiary winietowania przy różnych wartościach przysłony.61  
* **Przymykanie przysłony:** Jest to najskuteczniejsza metoda redukcji winietowania optycznego i często również pikselowego.60 Zazwyczaj przymknięcie przysłony o 1-2 stopnie EV od wartości maksymalnej znacząco zmniejsza lub eliminuje ten problem.  
* **Odpowiednie akcesoria:** Aby uniknąć winietowania mechanicznego, należy:  
  * Stosować filtry o cienkich oprawkach (typu "slim"), zwłaszcza przy obiektywach szerokokątnych.61  
  * Unikać jednoczesnego stosowania wielu filtrów.61  
  * Używać osłon przeciwsłonecznych dedykowanych do danego modelu obiektywu i prawidłowo je mocować.60  
* **Format matrycy/obiektywu:** Należy używać obiektywów przeznaczonych dla danego formatu matrycy. Na przykład, stosowanie obiektywu zaprojektowanego dla matrycy APS-C na aparacie pełnoklatkowym (bez włączonego trybu kadrowania w aparacie) spowoduje bardzo silne winietowanie (całkowite zaciemnienie brzegów kadru), ponieważ pole obrazowe takiego obiektywu jest zbyt małe, aby pokryć całą powierzchnię matrycy pełnoklatkowej.60

#### **Techniki korygowania winietowania w postprodukcji**

Jeśli winietowanie wystąpiło na zdjęciu, można je skorygować lub zredukować za pomocą oprogramowania do edycji zdjęć.

* **Automatyczna korekcja profilami obiektywów:** Większość zaawansowanych programów do wywoływania plików RAW (takich jak Adobe Lightroom, Camera Raw, DxO PhotoLab, Capture One) posiada wbudowane profile korekcyjne dla szerokiej gamy obiektywów.61 Te profile zawierają informacje o charakterystyce danego obiektywu, w tym o jego typowym winietowaniu przy różnych ogniskowych i przysłonach. Zastosowanie takiego profilu pozwala na automatyczną i zazwyczaj bardzo skuteczną korekcję winietowania, a także innych wad optycznych, takich jak dystorsja czy aberracja chromatyczna.  
* **Manualna korekcja:** Programy graficzne oferują również narzędzia do manualnej korekcji winietowania. Zazwyczaj są to suwaki pozwalające na rozjaśnienie brzegów kadru (suwak "Amount" lub "Siła"), określenie zasięgu korekcji (suwak "Midpoint" lub "Punkt środkowy") oraz płynności przejścia między skorygowanym a nieskorygowanym obszarem (suwak "Feather" lub "Wtapianie").61  
* **Winietowanie jako efekt artystyczny:** Czasami fotografowie celowo dodają winietowanie w postprodukcji (lub używają obiektywów generujących silne winietowanie), aby uzyskać określony efekt artystyczny.60 Delikatne przyciemnienie brzegów kadru może pomóc skupić uwagę widza na głównym motywie zdjęcia, dodać głębi lub nadać fotografii klimat retro.

Poniższa tabela systematyzuje informacje o różnych typach winietowania:

| Cecha | Winietowanie Optyczne/Naturalne | Winietowanie Mechaniczne | Winietowanie Pikselowe/Cyfrowe |
| :---- | :---- | :---- | :---- |
| **Główne przyczyny** | Prawo cos⁴θ, ograniczenia konstrukcyjne soczewek (średnica, wewnętrzne przesłanianie) 60 | Fizyczne blokowanie światła przez filtry, osłony przeciwsłoneczne, inne akcesoria 60 | Kątowa czułość pikseli, efektywność mikrosoczewek dla światła padającego pod kątem 60 |
| **Charakterystyczne objawy** | Płynny spadek jasności od centrum ku brzegom kadru 60 | Często gwałtowne zaciemnienie rogów, czasem z ostrymi krawędziami 60 | Płynny spadek jasności, potęgujący winietowanie optyczne; zależny od konstrukcji matrycy i obiektywu (telecentryczność) 60 |
| **Wpływ przysłony** | Znacząca redukcja przy przymknięciu 60 | Zwykle niewielki wpływ; może zmienić kształt zaciemnienia | Może być zredukowane przez przymykanie przysłony (zmniejszenie kątów padania światła) |
| **Metody zapobiegania (fotografowanie)** | Przymykanie przysłony, wybór obiektywu o niskim winietowaniu 60 | Stosowanie cienkich filtrów, unikanie stackowania, używanie dedykowanych osłon 61 | Używanie obiektywów telecentrycznych (jeśli to możliwe i uzasadnione) |
| **Metody korekcji (postprodukcja)** | Profile obiektywów, manualna korekcja jasności brzegów 61 | Kadrowanie zdjęcia, manualne rozjaśnianie (trudniejsze przy ostrych krawędziach) | Profile obiektywów (często korygowane łącznie z optycznym), manualna korekcja |

## **8\. Efekt dyfrakcji przy mocno zamkniętej przysłonie – dlaczego mocno zamknięta przysłona prowadzi do mniej ostrych zdjęć**

Jednym z paradoksów w fotografii jest fakt, że choć przymykanie przysłony generalnie zwiększa głębię ostrości i może poprawiać ostrość poprzez redukcję niektórych aberracji optycznych, zbyt mocne jej domknięcie (np. do wartości f/16, f/22, f/32 i mniejszych) prowadzi do zauważalnego spadku ogólnej ostrości obrazu.41 Zjawiskiem odpowiedzialnym za ten efekt jest dyfrakcja światła.

### **Wprowadzenie do dyfrakcji światła**

* **Natura falowa światła:** Aby zrozumieć dyfrakcję, należy przypomnieć, że światło, oprócz tego, że składa się z cząstek (fotonów), wykazuje również właściwości falowe.41 Jako fala elektromagnetyczna, światło podlega zjawiskom typowym dla fal, takim jak interferencja i właśnie dyfrakcja.  
* **Czym jest dyfrakcja:** Dyfrakcja to zjawisko fizyczne polegające na ugięciu się fali (w tym przypadku fali świetlnej) na krawędziach przeszkód lub podczas przechodzenia przez bardzo małe otwory.41 Zgodnie z zasadą Huygensa, każdy punkt na czole fali można traktować jako źródło nowej fali kulistej. Gdy fala napotyka przeszkodę lub wąską szczelinę, te wtórne fale interferują ze sobą, prowadząc do zmiany kierunku rozchodzenia się fali i jej "rozprzestrzeniania się" w obszarze cienia geometrycznego.  
* **Kiedy dyfrakcja staje się istotna w fotografii:** Zjawisko dyfrakcji jest obecne zawsze, gdy światło przechodzi przez otwór przysłony w obiektywie. Jednak jego wpływ na jakość obrazu staje się zauważalny i zaczyna ograniczać ostrość dopiero wtedy, gdy otwór przysłony jest bardzo mały – czyli przy wysokich wartościach liczbowych f (np. f/16, f/22 i więcej).45 Dzieje się tak, ponieważ stopień ugięcia fali jest tym większy, im mniejszy jest rozmiar otworu w stosunku do długości fali światła. Przy małych otworach przysłony, ugięte fale świetlne zaczynają znacząco interferować, prowadząc do rozmycia obrazu.

### **Wpływ dyfrakcji na jakość obrazu**

Głównym i najbardziej niepożądanym skutkiem dyfrakcji w fotografii jest spadek postrzeganej ostrości i utrata drobnych detali na zdjęciu.41

* **Rozmycie obrazu i spadek ostrości:** Z powodu dyfrakcji, punktowe źródło światła (np. bardzo odległa gwiazda lub bardzo mały detal na fotografowanym obiekcie) nie jest już odwzorowywane na matrycy jako idealny punkt, nawet jeśli obiektyw jest doskonale skorygowany pod względem aberracji. Zamiast tego, obraz punktu staje się rozmytą plamką, znaną jako krążek Airy'ego, otoczoną serią coraz słabszych koncentrycznych pierścieni dyfrakcyjnych.68 To rozmycie powoduje, że drobne szczegóły obrazu zlewają się ze sobą, a ogólna ostrość zdjęcia ulega pogorszeniu.41  
* **Jak dyfrakcja ogranicza zdolność rozdzielczą obiektywu:** Zdolność rozdzielcza układu optycznego to jego zdolność do odróżniania dwóch blisko siebie położonych punktów lub linii. Dyfrakcja narzuca fundamentalne fizyczne ograniczenie na maksymalną możliwą do osiągnięcia zdolność rozdzielczą przez dany obiektyw przy określonym otworze przysłony.70 Gdy krążki Airy'ego odpowiadające dwóm bliskim punktom obiektu zaczynają się na siebie znacząco nakładać z powodu dyfrakcji, punkty te przestają być rozróżnialne na obrazie, co oznacza spadek zdolności rozdzielczej.72

### **Krążek Airy’ego**

Pojęcie krążka Airy'ego jest kluczowe dla zrozumienia wpływu dyfrakcji na obrazowanie.

* **Obraz dyfrakcyjny punktu świetlnego:** W idealnym układzie optycznym, którego jedynym ograniczeniem jest dyfrakcja (tzn. pozbawionym aberracji), obraz punktowego źródła światła utworzony przez okrągłą aperturę (jaką w przybliżeniu jest otwór przysłony) nie jest matematycznym punktem. Jest to charakterystyczny wzór dyfrakcyjny, składający się z centralnej, jasnej plamki zwanej dyskiem (lub krążkiem) Airy'ego, która zawiera około 84% całkowitej energii światła, oraz otaczających ją koncentrycznych, coraz słabszych jasnych i ciemnych pierścieni dyfrakcyjnych.68  
* **Jak rozmiar krążka Airy’ego zależy od długości fali światła i wielkości otworu przysłony:** Średnica pierwszego ciemnego pierścienia dyfrakcyjnego (który ogranicza dysk Airy'ego) jest dana wzorem: d≈2.44⋅λ⋅(f/D) gdzie:  
  * d to średnica krążka Airy'ego na płaszczyźnie obrazu,  
  * λ to długość fali światła (np. dla światła zielonego ok. 550 nm),  
  * f to ogniskowa obiektywu,  
  * D to średnica otworu przysłony. Ponieważ N=f/D to liczba f (wartość przysłony), wzór można zapisać jako: d≈2.44⋅λ⋅N Z tego wzoru wynikają dwie ważne zależności:  
  * **Im mniejszy otwór przysłony (czyli większa liczba f, N), tym większy jest krążek Airy’ego**.68 Oznacza to, że przy mocnym przymykaniu przysłony obraz punktu staje się coraz bardziej rozmyty przez dyfrakcję.  
  * Im dłuższa jest fala światła (np. światło czerwone ma dłuższą falę niż światło niebieskie), tym większy jest krążek Airy’ego dla tej samej wartości przysłony. Oznacza to, że dyfrakcja może być nieco bardziej widoczna dla światła czerwonego niż niebieskiego.  
* **Granica dyfrakcyjna rozdzielczości (kryterium Rayleigha):** Aby dwa blisko siebie położone punkty świetlne mogły być rozróżnione na obrazie, ich krążki Airy'ego nie mogą się zbytnio na siebie nakładać. Zgodnie z kryterium Rayleigha, dwa punkty są uznawane za ledwo rozróżnialne, jeśli centrum krążka Airy'ego jednego punktu przypada na pierwszy ciemny pierścień dyfrakcyjny drugiego punktu.70 Gdy krążki Airy'ego są zbyt duże (z powodu małego otworu przysłony) i mocno się na siebie nakładają, detale obrazu zlewają się, a zdolność rozdzielcza systemu spada.

### **Praktyczne konsekwencje dyfrakcji**

Zrozumienie zjawiska dyfrakcji ma istotne implikacje praktyczne dla fotografów.

* **Dlaczego ekstremalne przymykanie przysłony (np. f/22, f/32) prowadzi do spadku ostrości, mimo teoretycznie dużej głębi ostrości:** Jak wcześniej omówiono, przymykanie przysłony zwiększa głębię ostrości poprzez zmniejszenie rozmiaru geometrycznych krążków rozproszenia dla obiektów znajdujących się poza płaszczyzną ostrości. Jednakże, jednocześnie, zgodnie z prawami dyfrakcji, przymykanie przysłony prowadzi do powiększania się krążka Airy'ego dla każdego punktu obrazu. Przy bardzo małych otworach przysłony (wysokich liczbach f), efekt rozmycia dyfrakcyjnego staje się na tyle duży, że dominuje nad korzyściami płynącymi ze zwiększonej głębi ostrości i prowadzi do ogólnego spadku ostrości na całym zdjęciu, nawet w płaszczyźnie idealnego zogniskowania.45  
* **Optymalna przysłona dla danego obiektywu (tzw. "sweet spot"):** Każdy obiektyw fotograficzny charakteryzuje się pewnym zakresem wartości przysłony, przy którym osiąga on swoją najlepszą ostrość i ogólną jakość obrazu. Jest to tzw. "sweet spot" (optymalny punkt pracy). Jego istnienie wynika z kompromisu między dwoma przeciwstawnymi zjawiskami:  
  * **Aberracje optyczne:** Różnego rodzaju niedoskonałości układu optycznego (np. aberracja sferyczna, chromatyczna, koma, astygmatyzm) są zazwyczaj najbardziej widoczne przy maksymalnie otwartej przysłonie. Przymykanie przysłony o 1-3 stopnie EV często prowadzi do znacznej redukcji tych aberracji i poprawy ostrości, szczególnie na brzegach kadru.56  
  * **Dyfrakcja:** Jak omówiono, wpływ dyfrakcji jest pomijalny przy dużych i średnich otworach przysłony, ale jej negatywny wpływ na ostrość gwałtownie narasta wraz z dalszym przymykaniem przysłony.41 "Sweet spot" znajduje się zazwyczaj w środkowym zakresie dostępnych wartości przysłony, np. f/5.6, f/8 lub f/11 dla wielu obiektywów pełnoklatkowych.40 Dokładna wartość optymalnej przysłony zależy od konkretnej konstrukcji obiektywu i można ją znaleźć w jego szczegółowych testach.  
* **Wpływ rozmiaru matrycy i gęstości pikseli na percepcję efektów dyfrakcji:**  
  * Na matrycach o bardzo dużej gęstości pikseli (czyli o bardzo małych rozmiarach pojedynczych pikseli), negatywny wpływ dyfrakcji na ostrość może stać się widoczny już przy nieco większych otworach przysłony (czyli mniejszych liczbach f) niż na matrycach o tej samej wielkości fizycznej, ale mniejszej liczbie pikseli (czyli większych pikselach). Dzieje się tak, ponieważ rozmiar krążka Airy'ego może szybciej osiągnąć rozmiar porównywalny z rozmiarem kilku pikseli, co prowadzi do utraty informacji o drobnych detalach.  
  * W przypadku aparatów z mniejszymi matrycami (np. APS-C, Mikro Cztery Trzecie, czy matryce w smartfonach), które z natury używają obiektywów o krótszych ogniskowych i często mają bardzo małe piksele, dyfrakcja może stać się czynnikiem ograniczającym ostrość już przy umiarkowanych wartościach przysłony (np. f/8-f/11).41 Wiele aparatów w smartfonach ma stałą, zoptymalizowaną wartość przysłony, aby uniknąć problemów z dyfrakcją przy jednoczesnym zapewnieniu dużej głębi ostrości.

Spadek ostrości spowodowany dyfrakcją przy małych otworach przysłony nie jest wynikiem wady czy złej jakości obiektywu, lecz fundamentalnym prawem fizyki falowej, któremu podlega światło.41 Każdy obiektyw, niezależnie od jego doskonałości i ceny, będzie wykazywał spadek ostrości spowodowany dyfrakcją przy dostatecznie małym otworze przysłony. Rozmiar krążka Airy'ego jest determinowany przez długość fali światła i efektywną średnicę otworu (liczbę f). Żaden projekt optyczny nie jest w stanie "obejść" tego zjawiska. Dlatego często mówi się o "granicy dyfrakcyjnej" jako teoretycznym maksimum rozdzielczości, jakie może osiągnąć dany układ optyczny przy danym otworze. Fotografowie muszą więc być świadomi, że dążenie do maksymalnej głębi ostrości poprzez ekstremalne przymykanie przysłony zawsze wiąże się z kompromisem w postaci utraty ogólnej ostrości obrazu.

Percepcja wpływu dyfrakcji zależy również od tego, jak rozmiar krążka Airy'ego ma się do rozmiaru pojedynczego piksela na matrycy.72 Jeśli krążek Airy'ego jest znacznie mniejszy niż rozmiar jednego piksela, to dyfrakcja nie jest głównym czynnikiem ograniczającym rozdzielczość systemu – ograniczeniem jest wówczas rozmiar piksela (zdolność matrycy do próbkowania obrazu). Jeśli jednak krążek Airy'ego staje się porównywalny lub większy od rozmiaru piksela (lub obejmuje kilka pikseli), to obraz jest "rozmyty przez dyfrakcję", a system osiągnął swoją granicę dyfrakcyjną. Dalsze zmniejszanie rozmiaru pikseli (zwiększanie ich gęstości) nie przyniesie już wzrostu rzeczywistej rozdzielczości przy tej wartości przysłony, ponieważ informacja o drobniejszych detalach jest tracona z powodu dyfrakcyjnego rozmycia, zanim dotrze do pikseli. Dla każdej matrycy (o określonym rozmiarze piksela) istnieje pewna wartość przysłony (tzw. "diffraction limited aperture" \- DLA), powyżej której (czyli przy mniejszych otworach/większych liczbach f) dyfrakcja zaczyna degradować obraz w stopniu większym niż wynikałoby to z samego rozmiaru piksela.

## **9\. Jak działa światło błyskowe**

Lampa błyskowa jest nieocenionym narzędziem w fotografii, pozwalającym na oświetlenie sceny w warunkach niedostatecznego światła zastanego, zamrożenie ruchu, a także kreatywne modelowanie światła i cienia. Zrozumienie zasady jej działania oraz kluczowych parametrów pozwala na pełne wykorzystanie jej możliwości.

### **Podstawy działania lampy błyskowej**

Sercem większości fotograficznych lamp błyskowych, od małych wbudowanych w aparaty kompaktowe po potężne studyjne jednostki, jest palnik ksenonowy i układ zasilający oparty na kondensatorze.31

* **Budowa palnika ksenonowego:** Palnik ksenonowy to zazwyczaj niewielka, prosta lub ukształtowana (np. w literę U) rurka wykonana ze szkła kwarcowego, wypełniona gazem szlachetnym – ksenonem – pod odpowiednio dobranym ciśnieniem. Na obu końcach rurki znajdują się główne elektrody (anoda i katoda), a często wokół rurki lub w jej pobliżu umieszczona jest dodatkowa elektroda wyzwalająca.31  
* **Rola kondensatora:** Kluczowym elementem układu zasilającego lampę błyskową jest kondensator o dużej pojemności. Jest on ładowany do stosunkowo wysokiego napięcia (kilkaset woltów) z baterii aparatu lub dedykowanego źródła zasilania lampy.31 Kondensator pełni rolę magazynu energii elektrycznej, która następnie zostanie gwałtownie rozładowana przez palnik w celu wygenerowania błysku.31  
* **Proces jonizacji gazu i emisji światła:** Działanie lampy błyskowej przebiega w kilku etapach:  
  1. **Ładowanie kondensatora głównego:** Po włączeniu lampy lub po poprzednim błysku, układ elektroniczny ładuje kondensator główny do wymaganego napięcia. Czas ładowania zależy od pojemności kondensatora, mocy źródła zasilania i stopnia rozładowania po poprzednim błysku.  
  2. **Impuls wyzwalający (trigger):** Gdy fotograf naciska spust migawki (lub gdy aparat wysyła sygnał synchronizacji), specjalny układ wyzwalający (zazwyczaj mały transformator impulsowy, tzw. cewka wyzwalająca) generuje bardzo krótki impuls o bardzo wysokim napięciu (rzędu kilku do kilkunastu kilowoltów).31 Ten impuls jest podawany na elektrodę wyzwalającą palnika.  
  3. **Jonizacja ksenonu:** Wysokonapięciowy impuls wyzwalający powoduje jonizację niewielkiej ilości gazu ksenonowego wewnątrz rurki palnika, tworząc w ten sposób przewodzącą ścieżkę (kanał plazmowy) między głównymi elektrodami.31 Zjonizowany gaz ma znacznie niższą rezystancję niż gaz w stanie neutralnym.  
  4. **Wyładowanie główne:** Utworzenie przewodzącego kanału w ksenonie pozwala na gwałtowne rozładowanie energii zgromadzonej w głównym kondensatorze przez palnik. Przez zjonizowany gaz przepływa prąd o dużym natężeniu. Ten przepływ prądu powoduje silne wzbudzenie atomów ksenonu, które następnie, wracając do stanu podstawowego, emitują bardzo jasny, krótkotrwały impuls światła.31 Czas trwania tego błysku jest bardzo krótki, typowo od około 1/1000 sekundy (dla pełnej mocy) do nawet 1/50000 sekundy lub krócej (dla niższych poziomów mocy w zaawansowanych lampach).74 Światło emitowane przez palnik ksenonowy ma szerokie spektrum, zbliżone do charakterystyki światła dziennego, co ułatwia uzyskanie naturalnych kolorów na zdjęciach.

### **Kluczowe parametry i pojęcia**

Aby efektywnie korzystać z lampy błyskowej, należy zrozumieć kilka kluczowych parametrów i pojęć.

#### **Liczba przewodnia (GN – Guide Number)**

Liczba przewodnia jest podstawowym parametrem określającym moc (a właściwie maksymalny zasięg efektywny) lampy błyskowej.75

* **Definicja:** Jest to wartość liczbowa, standardowo podawana dla czułości ISO 100 i określonego kąta rozsyłu światła przez palnik lampy (często odpowiadającego pokryciu pola widzenia dla obiektywu o ogniskowej 50 mm lub 105 mm na pełnej klatce).77 Liczba przewodnia (GN) jest zdefiniowana wzorem: GN=Odległosˊcˊ×Liczba\_f gdzie *Odległość* to dystans od lampy do oświetlanego obiektu (wyrażony w metrach lub stopach, w zależności od specyfikacji lampy), a *Liczba\_f* to wartość przysłony zapewniająca prawidłową ekspozycję przy ISO 100 i pełnej mocy błysku.79  
* **Jak wykorzystać GN:** Znajomość liczby przewodniej pozwala na manualne obliczenie prawidłowych ustawień ekspozycji:  
  * Aby obliczyć wymaganą wartość przysłony dla danej odległości od obiektu: Liczba\_f=GN/Odległosˊcˊ 79  
  * Aby obliczyć maksymalny efektywny zasięg błysku przy danej wartości przysłony: Odległosˊcˊ=GN/Liczba\_f 79  
* **Wpływ ISO na efektywną liczbę przewodnią:** Zwiększenie czułości ISO matrycy pozwala na użycie mniejszej mocy błysku (jeśli lampa ma regulację mocy) lub na oświetlenie obiektu znajdującego się w większej odległości. Efektywna liczba przewodnia (GN\_eff) rośnie wraz ze wzrostem czułości ISO. Zależność tę można przybliżyć wzorem: GNeff​=GNISO100​⋅(ISOaktualne​/ISO100​)​ Na przykład, podwojenie czułości ISO (np. z ISO 100 na ISO 200\) zwiększa efektywną liczbę przewodnią o czynnik 2​≈1.414. Oznacza to, że przy ISO 200 możemy użyć przysłony o jeden stopień mniejszej (np. f/5.6 zamiast f/4) lub oświetlić obiekt znajdujący się 1.4 raza dalej niż przy ISO 100, przy zachowaniu tej samej ekspozycji błysku.79

#### **Czas synchronizacji (X-sync)**

Czas synchronizacji, często oznaczany jako X-sync, jest kluczowym parametrem związanym z użyciem lampy błyskowej w aparatach z migawką szczelinową (najczęściej spotykaną w lustrzankach cyfrowych i wielu aparatach bezlusterkowych).74

* **Definicja:** Jest to najkrótszy czas otwarcia migawki, przy którym cała powierzchnia matrycy światłoczułej jest w pełni odsłonięta dokładnie w momencie, gdy lampa błyskowa emituje swój główny, krótkotrwały impuls światła.74 Migawka szczelinowa składa się z dwóch kurtyn (pierwszej i drugiej), które przesuwają się przed matrycą. Przy krótkich czasach naświetlania, druga kurtyna zaczyna zamykać szczelinę, zanim pierwsza kurtyna w pełni ją otworzy – szczelina o stałej szerokości przesuwa się wówczas wzdłuż matrycy. Czas X-sync to najkrótszy czas, przy którym szczelina jest na tyle szeroka, że na moment odsłania całą matrycę. Typowe wartości X-sync to 1/125 s, 1/200 s, 1/250 s, w zależności od modelu aparatu.75  
* **Konsekwencje użycia czasu naświetlania krótszego niż X-sync (bez trybu HSS):** Jeśli ustawimy w aparacie czas naświetlania krótszy niż jego natywny czas X-sync (a lampa i aparat nie obsługują trybu HSS, o którym mowa niżej), to w momencie błysku tylko część matrycy będzie odsłonięta. Skutkiem tego będzie zdjęcie, na którym część kadru (zazwyczaj poziomy pas) będzie prawidłowo naświetlona błyskiem, a reszta pozostanie ciemna (naświetlona tylko światłem zastanym) lub całkowicie czarna.

#### **Synchronizacja na pierwszą i drugą kurtynę migawki**

W przypadku używania czasów naświetlania dłuższych niż czas trwania błysku (co jest typową sytuacją), fotograf ma możliwość wyboru, w którym momencie długiej ekspozycji ma nastąpić błysk lampy.74

* **Synchronizacja na pierwszą kurtynę (Front-curtain sync):** Jest to standardowy tryb synchronizacji w większości aparatów. Lampa błyskowa wyzwalana jest natychmiast po pełnym otwarciu pierwszej kurtyny migawki (czyli na początku czasu naświetlania).74 Jeśli fotografujemy poruszający się obiekt przy długim czasie naświetlania, efekt będzie taki, że obiekt zostanie "zamrożony" przez błysk na początku swojej drogi, a następnie zarejestrowane zostaną smugi jego ruchu powstałe w świetle zastanym. Te smugi będą znajdować się **przed** zamrożonym obrazem obiektu, co często wygląda nienaturalnie.74  
* **Synchronizacja na drugą kurtynę (Rear-curtain sync):** W tym trybie lampa błyskowa wyzwalana jest tuż przed zamknięciem drugiej kurtyny migawki (czyli pod koniec czasu naświetlania) \[74, S\_B

#### **Works cited**

1. Jak działa aparat cyfrowy? Proste wyjaśnienie budowy i zasad ..., accessed June 6, 2025, [https://epkrspotters.pl/jak-dziala-aparat-cyfrowy-proste-wyjasnienie-budowy-i-zasad-dzialania](https://epkrspotters.pl/jak-dziala-aparat-cyfrowy-proste-wyjasnienie-budowy-i-zasad-dzialania)  
2. Matryce CMOS/CCD \- Avicon, accessed June 6, 2025, [https://avicon.pl/dzialalnoscbr/technologie-wizyjne/cmos-ccd/](https://avicon.pl/dzialalnoscbr/technologie-wizyjne/cmos-ccd/)  
3. Astronomical Cameras \- Las Cumbres Observatory, accessed June 6, 2025, [https://lco.global/spacebook/telescopes/cameras/](https://lco.global/spacebook/telescopes/cameras/)  
4. Introduction to CMOS Image Sensors \- Evident Scientific, accessed June 6, 2025, [https://evidentscientific.com/en/microscope-resource/knowledge-hub/digital-imaging/cmosimagesensors](https://evidentscientific.com/en/microscope-resource/knowledge-hub/digital-imaging/cmosimagesensors)  
5. Understanding Image Sensors: The Semiconductor Behind Our Memories | Galaxy.ai, accessed June 6, 2025, [https://galaxy.ai/youtube-summarizer/understanding-image-sensors-the-semiconductor-behind-our-memories-Lgm-CnfWiTI](https://galaxy.ai/youtube-summarizer/understanding-image-sensors-the-semiconductor-behind-our-memories-Lgm-CnfWiTI)  
6. PHYSICS Photo Diode | PDF | Diode | P–N Junction \- Scribd, accessed June 6, 2025, [https://www.scribd.com/presentation/645402623/PHYSICS-Photo-diode](https://www.scribd.com/presentation/645402623/PHYSICS-Photo-diode)  
7. Photodiode Characteristics And Applications Photodiode, accessed June 6, 2025, [https://beta.mercycollege.edu/fetch.php/libweb/4000032/PhotodiodeCharacteristicsAndApplicationsPhotodiode.pdf](https://beta.mercycollege.edu/fetch.php/libweb/4000032/PhotodiodeCharacteristicsAndApplicationsPhotodiode.pdf)  
8. PHOTODIODE BASICS \- Wavelength Electronics, accessed June 6, 2025, [https://www.teamwavelength.com/photodiode-basics/](https://www.teamwavelength.com/photodiode-basics/)  
9. Photodiode Characteristics and Applications \- MIT, accessed June 6, 2025, [http://web.mit.edu/6.101/www/reference/Photodiode\_Characteristics.pdf](http://web.mit.edu/6.101/www/reference/Photodiode_Characteristics.pdf)  
10. Characteristics and Use of Photodiodes, accessed June 6, 2025, [https://www.chem.uci.edu/\~unicorn/243/handouts/photodiode.pdf](https://www.chem.uci.edu/~unicorn/243/handouts/photodiode.pdf)  
11. Photodiode PDF | PDF | Diode | P–N Junction \- Scribd, accessed June 6, 2025, [https://www.scribd.com/document/390897394/photodiode-pdf](https://www.scribd.com/document/390897394/photodiode-pdf)  
12. Matryca CCD – Wikipedia, wolna encyklopedia, accessed June 6, 2025, [https://pl.wikipedia.org/wiki/Matryca\_CCD](https://pl.wikipedia.org/wiki/Matryca_CCD)  
13. Porównanie matryc CCD i CMOS \- Fotografia cyfrowa poradnik, accessed June 6, 2025, [http://www.fotoporadnik.pl/porownanie-matryc-2.html](http://www.fotoporadnik.pl/porownanie-matryc-2.html)  
14. Photodiode | PPT \- SlideShare, accessed June 6, 2025, [https://www.slideshare.net/slideshow/photodiode-58931332/58931332](https://www.slideshare.net/slideshow/photodiode-58931332/58931332)  
15. CCD vs CMOS Image Sensors: A Comprehensive Guide for ..., accessed June 6, 2025, [https://www.wevolver.com/article/ccd-vs-cmos-image-sensors](https://www.wevolver.com/article/ccd-vs-cmos-image-sensors)  
16. Matryce CCD i CMOS \- Dyskusje o sprzęcie \- Astropolis ..., accessed June 6, 2025, [https://astropolis.pl/topic/54830-matryce-ccd-i-cmos/](https://astropolis.pl/topic/54830-matryce-ccd-i-cmos/)  
17. Dynamic Range \- Evident Scientific, accessed June 6, 2025, [https://evidentscientific.com/en/microscope-resource/knowledge-hub/digital-imaging/concepts/dynamicrange](https://evidentscientific.com/en/microscope-resource/knowledge-hub/digital-imaging/concepts/dynamicrange)  
18. Pattern Noise: DSNU and PRNU | Teledyne Vision Solutions, accessed June 6, 2025, [https://www.teledynevisionsolutions.com/learn/learning-center/imaging-fundamentals/pattern-noise-dsnu-and-prnu/](https://www.teledynevisionsolutions.com/learn/learning-center/imaging-fundamentals/pattern-noise-dsnu-and-prnu/)  
19. How a Charge Coupled Device (CCD) Image ... \- Teledyne Imaging, accessed June 6, 2025, [https://www.teledyneimaging.com/media/1300/2020-01-22\_e2v\_how-a-charge-coupled-device-works\_web.pdf](https://www.teledyneimaging.com/media/1300/2020-01-22_e2v_how-a-charge-coupled-device-works_web.pdf)  
20. Kwalifikacja E.12. Montaż i eksploatacja komputerów osobistych oraz urządzeń peryferyjnych. Podręcznik do nauki zawodu tech, accessed June 6, 2025, [https://tiqcmc.webwave.dev/lib/tiqcmc/Kwalifikacja\_e12\_podrecznik\_do\_nauki\_zawodu\_tech\_informatyk-ka5dpz5o.pdf](https://tiqcmc.webwave.dev/lib/tiqcmc/Kwalifikacja_e12_podrecznik_do_nauki_zawodu_tech_informatyk-ka5dpz5o.pdf)  
21. Matryce światłoczułe – właściwości, parametry, zastosowania \- SIN PUT \- Politechnika Poznańska, accessed June 6, 2025, [https://sin.put.poznan.pl/files/download/34623](https://sin.put.poznan.pl/files/download/34623)  
22. CCD vs CMOS \- Matryce CCD i ich działanie \- Optyczne.pl, accessed June 6, 2025, [https://www.optyczne.pl/14.2-artyku%C5%82-CCD\_vs\_CMOS\_Matryce\_CCD\_i\_ich\_dzia%C5%82anie.html](https://www.optyczne.pl/14.2-artyku%C5%82-CCD_vs_CMOS_Matryce_CCD_i_ich_dzia%C5%82anie.html)  
23. Full Well Capacity and Pixel Saturation | Teledyne Vision Solutions, accessed June 6, 2025, [https://www.teledynevisionsolutions.com/learn/learning-center/imaging-fundamentals/full-well-capacity-and-pixel-saturation/](https://www.teledynevisionsolutions.com/learn/learning-center/imaging-fundamentals/full-well-capacity-and-pixel-saturation/)  
24. (PDF) Semiconductor Image Sensing \- ResearchGate, accessed June 6, 2025, [https://www.researchgate.net/publication/50434059\_Semiconductor\_Image\_Sensing](https://www.researchgate.net/publication/50434059_Semiconductor_Image_Sensing)  
25. Budowa i działanie matrycy typu CMOS \- Fotografia cyfrowa poradnik, accessed June 6, 2025, [https://www.fotoporadnik.pl/matryca-cmos-1.html](https://www.fotoporadnik.pl/matryca-cmos-1.html)  
26. Budowa aparatu cyfrowego, cześć II \- MATRYCA. 6\. O parametrach ..., accessed June 6, 2025, [https://www.benchmark.pl/testy\_i\_recenzje/budowa-aparatu-cyfrowego-czesc-ii-matryca-2631/strona/8059.html](https://www.benchmark.pl/testy_i_recenzje/budowa-aparatu-cyfrowego-czesc-ii-matryca-2631/strona/8059.html)  
27. Jak uzyskać efekt bokeh na zdjęciu \- szybkie wskazówki, accessed June 6, 2025, [https://fotografiadlaciekawych.pl/index.php/2023/10/04/szybkie-wskazowki-jak-uzyskac-efekt-bokeh-na-zdjeciu/](https://fotografiadlaciekawych.pl/index.php/2023/10/04/szybkie-wskazowki-jak-uzyskac-efekt-bokeh-na-zdjeciu/)  
28. Depth of field \- Wikipedia, accessed June 6, 2025, [https://en.wikipedia.org/wiki/Depth\_of\_field](https://en.wikipedia.org/wiki/Depth_of_field)  
29. Zrozumienie DPI i jego wpływu na jakość obrazu \- Vertipen, accessed June 6, 2025, [https://vertipen.pl/zrozumienie-dpi-i-jego-wplywu-na-jakosc-obrazu/](https://vertipen.pl/zrozumienie-dpi-i-jego-wplywu-na-jakosc-obrazu/)  
30. Co to jest gęstość pikseli? Szczegółowy przewodnik \- YUCHIP, accessed June 6, 2025, [https://www.yuchip-led.com/pl/co-to-jest-g%C4%99sto%C5%9B%C4%87-pikseli---szczeg%C3%B3%C5%82owy-przewodnik/](https://www.yuchip-led.com/pl/co-to-jest-g%C4%99sto%C5%9B%C4%87-pikseli---szczeg%C3%B3%C5%82owy-przewodnik/)  
31. Obwód lampy błyskowej ksenonowej: Jak zbudować obwód \- PCB, accessed June 6, 2025, [https://ourpcb.pl/blyskowej-ksenonowej.html](https://ourpcb.pl/blyskowej-ksenonowej.html)  
32. PIXEL SIZE & SENSITIVITY \- Photon Lines Ltd, accessed June 6, 2025, [https://photonlines.co.uk/wp-content/uploads/2020/07/kb\_pixel\_size\_sensitivity\_105.pdf](https://photonlines.co.uk/wp-content/uploads/2020/07/kb_pixel_size_sensitivity_105.pdf)  
33. Image Sensor Noise – measurement and modeling | Imatest, accessed June 6, 2025, [https://www.imatest.com/imaging/image-sensor-noise/](https://www.imatest.com/imaging/image-sensor-noise/)  
34. Image noise \- Wikipedia, accessed June 6, 2025, [https://en.wikipedia.org/wiki/Image\_noise](https://en.wikipedia.org/wiki/Image_noise)  
35. Noise | Imatest, accessed June 6, 2025, [https://www.imatest.com/imaging/noise/](https://www.imatest.com/imaging/noise/)  
36. NOISE ANALYSIS IN CMOS IMAGE SENSORS \- Stanford University, accessed June 6, 2025, [https://isl.stanford.edu/\~abbas/group/papers\_and\_pub/hui\_thesis.pdf](https://isl.stanford.edu/~abbas/group/papers_and_pub/hui_thesis.pdf)  
37. Aparaty i kamery \- afterdusk.pl :: Porady, accessed June 6, 2025, [https://www.afterdusk.pl/index.php?sec=art\&doc=basic04%3A4](https://www.afterdusk.pl/index.php?sec=art&doc=basic04:4)  
38. Test Sony A7C II \- Zakres i dynamika tonalna \- Test aparatu \- Optyczne.pl, accessed June 6, 2025, [https://www.optyczne.pl/504.8-Test\_aparatu-Sony\_A7C\_II\_Zakres\_i\_dynamika\_tonalna.html](https://www.optyczne.pl/504.8-Test_aparatu-Sony_A7C_II_Zakres_i_dynamika_tonalna.html)  
39. Do czego służy i jak działa przysłona? \- fotografia cyfrowa i analogowa, edycja obrazu, pojęcia i techniki fotograficzne, recenzje, testy aparatów \- Fotografuj.pl, accessed June 6, 2025, [http://www.fotografuj.pl/Article/Przyslona\_irysowa\_otwor\_wzgledny\_liczba\_wartosc\_przyslony/id/78/page/2](http://www.fotografuj.pl/Article/Przyslona_irysowa_otwor_wzgledny_liczba_wartosc_przyslony/id/78/page/2)  
40. Przysłona w Aparacie | Poradnik Dla Początkujących 2024 \- Waskiel.pl, accessed June 6, 2025, [https://waskiel.pl/przyslona-w-aparacie/](https://waskiel.pl/przyslona-w-aparacie/)  
41. Przysłona w aparacie \- poradnik obsługi aparatu fotograficznego, accessed June 6, 2025, [https://fotografiadlaciekawych.pl/index.php/2022/10/12/przyslona-w-aparacie-poradnik-obslugi-aparatu-fotograficznego/](https://fotografiadlaciekawych.pl/index.php/2022/10/12/przyslona-w-aparacie-poradnik-obslugi-aparatu-fotograficznego/)  
42. Przysłona \- iZabezpieczenia.pl, accessed June 6, 2025, [https://www.izabezpieczenia.pl/kompendium-wiedzy/biblioteka-wiedzy/przyslona/](https://www.izabezpieczenia.pl/kompendium-wiedzy/biblioteka-wiedzy/przyslona/)  
43. What is f-stop on a camera? | F-stop photography \- Adobe, accessed June 6, 2025, [https://www.adobe.com/creativecloud/photography/discover/f-stop.html](https://www.adobe.com/creativecloud/photography/discover/f-stop.html)  
44. Czym jest trójkąt ekspozycji? Jak go zrozumieć i dobrze ustawić ..., accessed June 6, 2025, [https://fotoforma.pl/blog/czym-jest-trojkat-ekspozycji-jak-ustawic-aparat/](https://fotoforma.pl/blog/czym-jest-trojkat-ekspozycji-jak-ustawic-aparat/)  
45. Ustawienia aparatu do fotografii produktowej dla e-commerce \- Orbitvu, accessed June 6, 2025, [https://orbitvu.pl/blog/ustawienia-aparatu-do-fotografii-produktowej/](https://orbitvu.pl/blog/ustawienia-aparatu-do-fotografii-produktowej/)  
46. Aperture and F-Stops Explained \- Outdoor Photography School, accessed June 6, 2025, [https://www.outdoorphotographyschool.com/aperture-and-f-stops-explained/](https://www.outdoorphotographyschool.com/aperture-and-f-stops-explained/)  
47. Głębia Ostrości w Fotografii | Poradnik Dla Początkujących 2025 \- Waskiel.pl, accessed June 6, 2025, [https://waskiel.pl/glebia-ostrosci-co-to-jest/](https://waskiel.pl/glebia-ostrosci-co-to-jest/)  
48. Depth of Field and Depth of Focus | Edmund Optics, accessed June 6, 2025, [https://www.edmundoptics.com/knowledge-center/application-notes/imaging/depth-of-field-and-depth-of-focus/](https://www.edmundoptics.com/knowledge-center/application-notes/imaging/depth-of-field-and-depth-of-focus/)  
49. Understanding Depth of Field in Photography \- Cambridge in Colour, accessed June 6, 2025, [https://www.cambridgeincolour.com/tutorials/depth-of-field.htm](https://www.cambridgeincolour.com/tutorials/depth-of-field.htm)  
50. www.studiobinder.com, accessed June 6, 2025, [https://www.studiobinder.com/blog/what-is-circle-of-confusion-photography/\#:\~:text=The%20circle%20of%20confusion%20is%20what%20defines%20what's%20in%20or,circle%2C%20the%20sharper%20the%20image.](https://www.studiobinder.com/blog/what-is-circle-of-confusion-photography/#:~:text=The%20circle%20of%20confusion%20is%20what%20defines%20what's%20in%20or,circle%2C%20the%20sharper%20the%20image.)  
51. Understanding the Circle of Confusion in Photography, accessed June 6, 2025, [https://whosaidphotography.com/circle-of-confusion-in-photography/](https://whosaidphotography.com/circle-of-confusion-in-photography/)  
52. Circle of confusion \- Wikipedia, accessed June 6, 2025, [https://en.wikipedia.org/wiki/Circle\_of\_confusion](https://en.wikipedia.org/wiki/Circle_of_confusion)  
53. Głębia Ostrości \- poradnik dla początkujących fotografów, accessed June 6, 2025, [https://baronphotography.eu/glebia-ostrosci/](https://baronphotography.eu/glebia-ostrosci/)  
54. Głębia ostrości dla początkujących \- Szeroki Kadr, accessed June 6, 2025, [https://www.szerokikadr.pl/poradnik/glebia-ostrosci-fotograficzny-srodek-wyrazu](https://www.szerokikadr.pl/poradnik/glebia-ostrosci-fotograficzny-srodek-wyrazu)  
55. Co to jest bokeh? \- Foto \- Plus, accessed June 6, 2025, [https://fotoplus.pl/artykuly/co-to-jest-bokeh](https://fotoplus.pl/artykuly/co-to-jest-bokeh)  
56. Jak wybrać przysłonę? Co oznaczają wartości "f"? Kiedy zdjęcie jest najostrzejsze?, accessed June 6, 2025, [https://www.youtube.com/watch?v=PAZlWTMgvnQ](https://www.youtube.com/watch?v=PAZlWTMgvnQ)  
57. Poznaj i zrozum działenie przysłony \- Digital Camera Polska, accessed June 6, 2025, [https://m.digitalcamerapolska.pl/warsztat/2908-poznaj-i-zrozum-dzialenie-przyslony](https://m.digitalcamerapolska.pl/warsztat/2908-poznaj-i-zrozum-dzialenie-przyslony)  
58. Przysłona w aparacie. Co to jest przepona? Jak ustawić przysłonę. | Szczęśliwy, accessed June 6, 2025, [https://radojuva.com/pl/2012/02/diafragma/](https://radojuva.com/pl/2012/02/diafragma/)  
59. Koło EV – kalkulator ekwiwalentu \- zts.SKIBEK, accessed June 6, 2025, [https://www.zts.skibek.pl/koloev-kalkulator-ekwiwalentu/](https://www.zts.skibek.pl/koloev-kalkulator-ekwiwalentu/)  
60. Fotografia od A do Z: Winietowanie \- Swiatobrazu.pl, accessed June 6, 2025, [https://www.swiatobrazu.pl/fotografia-od-a-do-z-winietowanie-23219.html](https://www.swiatobrazu.pl/fotografia-od-a-do-z-winietowanie-23219.html)  
61. Winietowanie w fotografii \- co to jest i co je powoduje?, accessed June 6, 2025, [https://tylkofotografia.pl/winietowanie/](https://tylkofotografia.pl/winietowanie/)  
62. Wady optyki, czyli nie taki diabeł straszny… | Fotopolis.pl, accessed June 6, 2025, [https://www.fotopolis.pl/temat-miesiaca/optyka/31157-wady-optyki-czyli-nie-taki-diabel-straszny](https://www.fotopolis.pl/temat-miesiaca/optyka/31157-wady-optyki-czyli-nie-taki-diabel-straszny)  
63. Jak działa obiektyw \- Szeroki Kadr, accessed June 6, 2025, [https://www.szerokikadr.pl/poradnik/jak-to-dziala-czesc-2-optyka](https://www.szerokikadr.pl/poradnik/jak-to-dziala-czesc-2-optyka)  
64. Na czym polega winietowanie w fotografii? \- Magazyn Ceneo.pl, accessed June 6, 2025, [https://magazyn.ceneo.pl/artykuly/winietowanie](https://magazyn.ceneo.pl/artykuly/winietowanie)  
65. Do czego służy osłona przeciwsłoneczna i jak ją wybrać | Porównywarka cen E-Katalog, accessed June 6, 2025, [https://e-katalog.pl/post/812/458\_dlya\_chego\_nuzhna\_blenda\_na\_obektiv\_i\_kak\_ee\_vybrat/](https://e-katalog.pl/post/812/458_dlya_chego_nuzhna_blenda_na_obektiv_i_kak_ee_vybrat/)  
66. Filtr Kenko Celeste UV \- recenzja \- Fotograf ślubny Marek Czeżyk, accessed June 6, 2025, [https://czezyk.pl/kenko-celeste-uv/](https://czezyk.pl/kenko-celeste-uv/)  
67. Retuszowanie i poprawianie zdjęć w programie Photoshop Elements \- Adobe Support, accessed June 6, 2025, [https://helpx.adobe.com/pl/photoshop-elements/using/retouching-correcting.html](https://helpx.adobe.com/pl/photoshop-elements/using/retouching-correcting.html)  
68. Dyfrakcja w fotografii: Co to jest i jak jej uniknąć, aby zdjęcia były ..., accessed June 6, 2025, [https://www.slowik.eu/dyfrakcja-w-fotografii-co-to-jest-i-jak-jej-uniknac/](https://www.slowik.eu/dyfrakcja-w-fotografii-co-to-jest-i-jak-jej-uniknac/)  
69. Przysłona w fotografii krajobrazowej. Jaką wybrać? \- Waskiel.pl, accessed June 6, 2025, [https://waskiel.pl/jaka-jest-najlepsza-przyslona-do-fotografii-krajobrazowej/](https://waskiel.pl/jaka-jest-najlepsza-przyslona-do-fotografii-krajobrazowej/)  
70. Zrozumienie apertury numerycznej w układach optycznych, accessed June 6, 2025, [https://chineselens.com/pl/understanding-numerical-aperture/](https://chineselens.com/pl/understanding-numerical-aperture/)  
71. PTMA o. Śląski \- Porady, accessed June 6, 2025, [https://www.slaski.ptma.pl/old/porady.html](https://www.slaski.ptma.pl/old/porady.html)  
72. IC 1396 Trąba Słonia \- Głęboki Kosmos (DS) \- Astropolis \- Astronomia i Astrofotografia, accessed June 6, 2025, [https://astropolis.pl/topic/33072-ic-1396-tr%C4%85ba-s%C5%82onia/](https://astropolis.pl/topic/33072-ic-1396-tr%C4%85ba-s%C5%82onia/)  
73. Lampy ksenonowe – działanie i dozbrajanie \- forvia hella, accessed June 6, 2025, [https://www.hella.com/techworld/pl/Technologia/Oswietlenie-baza-wiedzy-technicznej-i-praktycznych-porad/Lampy-ksenonowe-218/](https://www.hella.com/techworld/pl/Technologia/Oswietlenie-baza-wiedzy-technicznej-i-praktycznych-porad/Lampy-ksenonowe-218/)  
74. Synchronizacja błysku lampy \- Fotografia cyfrowa poradnik, accessed June 6, 2025, [http://www.fotoporadnik.pl/synchronizacja-lampy-blyskowe.html](http://www.fotoporadnik.pl/synchronizacja-lampy-blyskowe.html)  
75. Jaką lampę błyskową kupić? Porównanie i różnice – Blog Fripers.pl, accessed June 6, 2025, [https://fripers.pl/blog/?p=2309](https://fripers.pl/blog/?p=2309)  
76. Stroboss 36 \- Quadralite, accessed June 6, 2025, [https://www.quadralite.pl/stroboss-lampy/303-quadralite-stroboss-36](https://www.quadralite.pl/stroboss-lampy/303-quadralite-stroboss-36)  
77. image-acquire.com, accessed June 6, 2025, [https://image-acquire.com/guide-number/\#:\~:text=To%20calculate%20the%20GN%2C%20you,(10m%20multiplied%20by%204).](https://image-acquire.com/guide-number/#:~:text=To%20calculate%20the%20GN%2C%20you,\(10m%20multiplied%20by%204\).)  
78. www.michaelscamerahire.com.au, accessed June 6, 2025, [https://www.michaelscamerahire.com.au/resources/understanding-guide-numbers-gn\#:\~:text=Guide%20Number%20%3D%20Subject%20Distance%20from%20Flash%20%C3%97%20f%2Dstop\&text=Take%20the%20Canon%20600EX%20II,called%20the%20flash%20'zoom'.](https://www.michaelscamerahire.com.au/resources/understanding-guide-numbers-gn#:~:text=Guide%20Number%20%3D%20Subject%20Distance%20from%20Flash%20%C3%97%20f%2Dstop&text=Take%20the%20Canon%20600EX%20II,called%20the%20flash%20'zoom'.)  
79. Guide Number Secrets: Enhance Your Flash Photography Today, accessed June 6, 2025, [https://image-acquire.com/guide-number/](https://image-acquire.com/guide-number/)