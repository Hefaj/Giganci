
# Table of Contents

1.  [Zadanka<code>[1/4]</code>](#org69caf6a)


<a id="org69caf6a"></a>

# TODO Zadanka<code>[1/4]</code>

1.  [-] Konsola <code>[3/14]</code>
    1.  [X] Silnia
        -   Obliczyć silnie z liczny n.
        -   Problem:
            -   Jak się liczy silnie?
        -   Podpowiedz:
            -   !n = 1 \* 2 \* .. \* n
    
    2.  [X] Lotto
        -   Generowanie 6-ciu liczb z zakresu 1-49 bez powtórzeń.
        -   Problem:
            -   Jak losować bez powtórzeń?
        -   Podpowiedz:
            -   Tablica z liczbami 1,2,&#x2026;, 49 
                wymieszać i wyświetlić pierwsze 6
            -   int tablica = new int[49];
            -   optymalne rozwiązanie
    
    3.  [ ] Liczba Eulera
        -   Napisać program liczący przybliżenie liczby Eulera
        -   Problem:
            -   Co to jest liczba Eulera, jak ją liczyć?
        -   Podpowiedz:
            -   e = sum(1/n!) czyli 1/0! + 1/1! + 1/2! + &#x2026;
            -   zrobić z silni funkcje
            -   static int silnia(n){\`[liczenie]\`  return s}
        -   Rozwiązanie:
            -   for(i=0;i<n;i++)
                s+=1f/silnia(n)
    
    4.  [ ] Liczby pierwsze
        -   Wyświetlić wszystkie liczby pierwsze z przedziału od 2 do n.
        -   Problem:
            -   Co to jest liczba pierwsza?
            -   Jak sprawdzić czy liczba jest pierwsza?
        -   Podpowiedz:
            -   Znając liczbę pierwszą można wykluczyć jej wielokrotności.
    
    5.  [ ] Rozpisanie liczby
        -   Podając liczbę, ma zostać ona wyświetlona w postaci sumy liczb.
            1234 = 1000 + 200 + 30 + 4
        -   Problem:
            -   Jak przechwycić pojedyncze cyfry?
        -   Podpowiedz:
            -   string to tablica charów 
                string liczba = "1234";
                liczba[0] => "1";
            -   stringi można sklejać za pomocą znaku "+"
                "ala" + "ma" + "kota" => "alamakota"
    
    6.  [ ] Pochodna w punkcie
        -   Mając funkcje f(x) podać wartość pochodnej tej funkcji
            w wyznaczonym punkcie.
        -   Problem:
            -   Co to jest pochodna?
            -   Jak zakodować wzór pochodnej?
        -   Podpowiedz:
            -   Wyprowadzenie wzoru na pochodną ze wzoru Taylora
    
    7.  [X] Wyświetlanie choinki
        -   Za pomocą pętli wyświetlić trójkąt prostokątny z '\*' 
            dla danego n.
        -   Problem:
            -   BRAK
        -   Podpowiedz:
            -   np. n = 3
                -   .
                -   ..
                -   &#x2026;
    
    8.  [ ] Sortowanie tablicy liczb całkowitych
        -   Posortowanie rosnąco tablice liczb całkowitych.
        -   Problem:
            -   Jak wydajnie poukładać cyfry na swoich miejscach
        -   Podpowiedz:
            -   Array.Sort(array);
    
    9.  [ ] Liczba doskonała
        -   Sprawdzić czy podana liczba jest liczbą doskonałą.
        -   Problem:
            -   Co to jest liczba doskonała?
            -   Jak sprawdzić czy podana liczba jest liczbą doskonałą?
        -   Podpowiedz:
            -   dzielniki liczby 6 to 1, 2 i 3 czyli 1+2+3 = 6, 
                liczba 6 jest liczbą doskonałą (28, 496 tez)
            -   każda liczba dzieli się przez 1
            -   znajdź wszystkie dzielniki podanej liczby i zapisuj je do tablicy
    
    10. [ ] Złota liczba
        -   Podaj wartość złotej liczby.
        -   Problem:
            -   Co to jest złota liczba?
        -   Podpowiedz:
               1+1
              1+2
             2+3
            3+5
    
    11. [ ] Miejsce zerowe funkcji
        -   Mając funkcje f(x) chcemy znaleźć miejsce zerowe z przedziału <a,b>
        -   Problem:
            -   Jak?
        -   Podpowiedz:
            -   Metoda bisekcji
    
    12. [ ] Całka Riemanna (oznaczona)
        -   Mając f(x) policzyć całkę Riemanna na przedziale <a,b>.
        -   Problem:
            -   Na czym polega całkowanie?
        -   Podpowiedz:
            -   Metoda Trapezów
                Pole trapezu => (a+b)\*h/2
                Sprawdzić całkowanie dla f(x)=2x xe0..1
    
    13. [ ] Perceptron
        -   Stworzyć perceptron 2 wejścia 1 wyjście.
        -   Problem:
            -   Co to jest perceptron (neuron matematyczny).
        -   Podpowiedz:
            -   Algebra liniowa
                x <- wektor wejściowy
                w <- wektor wag
                Q <- Funkcja progowa unipolarna 
                     czyli 0 dla <0 i 1 dla >=0
                T <- Transponowanie
                
                    x1       w1
                x =     w =   
                    x2       w2
                
                y = Q( T(x)\*w )
                w <- losowe z przedziału (0,1)
    
    14. [ ] Uczenie perceptronu
        -   Stworzyć algorytm uczenia perceptrony
            Czyli modyfikacji wag (w) aby zwracało co chcemy
        -   Problem:
            -   W jaki sposób modyfikować wagi?
        -   Podpowiedz:
            -   Mając wynik (y) dla wektora uczącego x, x={x1,x2}
                i oczekując od perceptronu wyjścia y' dla wektora x.
                
                Możemy sprawdzić czy y'-y = 0
                jeżeli tak to znaczy, że perceptron
                zwraca poprawne wartości.
                
                Jeżeli nie to modyfikujemy wagi
                w1 += (y'-y)\*

2.  [-] WinForms <code>[7/9]</code>
    1.  [X] Napis 
        -   Program który pozwala wybrać z listy wielkość napisu.
            I zmienia rozmiar napisu na jaki wybraliśmy.
        -   Problem:
            -   Jak zmieniać rozmiar napisu?
            -   Jak zrobić rozwijalną liste?
        -   Podpowiedz:
            -   label.Font = new Font("Arial", 20); 20 <- rozmiar
            -   ToolBox - > ComboBox
            -   ComboBox -> events -> SelectedIndexChanged
    
    2.  [X] Pora roku
        -   Podajemy numer miesiąca a program mówi jak to pora roku.
            Grudzień (12) - Luty     (2)  - Zima
            Marzec   (3)  - Maj      (5)  - Wiosna
            Czerwiec (6)  - Sierpień (8)  - Lato
            Wrzesień (9)  - Listopad (11) - Jesień
        -   Podpowiedz:
            -   switch (n)
                case 3:
                case 4:
                case 5:
                    MessageBox.Show();
                    break;
    
    3.  [X] Liczba parzysta
        -   Program sprawdzający czy wpisana liczba jest liczbą parzystką.
        -   Problem:
            -   Kiedy liczba jest parzysta?
        -   Podpowiedz:
            -   Liczba jest parzysta jeżeli reszta z dzielenia przez 2 jest równa 0.
    
    4.  [X] Uciekający textbox
        -   Po najechaniu myszą textbox ucieka w inne 
            losowe miejsce w naszym oknie.
        -   Problem:
            -   Jaka funkcja jest wykonywana po najechaniu na element?
            -   Jak wylosować liczbę z odpowiedniego przedziału?
            -   Jak zmienić z pozycji kodu pozycję textboxa?
        -   Podpowiedz:
            -   Piorunek nad właściwościami.
            -   Random r = new Random();
                r.Next(a,b);
            -   box.location = new Point(x,y);
    
    5.  [X] Dynamiczna zmiana koloru checkbox-a
        -   Wpisując w textbox-a ma się znieniać kolor tła.
        -   Problem:
            -   Jak zmieniać kolor tła?
        -   Podpowiedz:
            -   this.BackColor = Color.FromArgb(r,g,b);
    
    6.  [ ] Oczopląs
        -   Migający form na losowe kolory
        -   Problem:
            -   W jaki sposób komputer "rozumie" kolory, jak się je przedstawia, [RGB](https://pl.wikipedia.org/wiki/RGB), [CMYK](https://pl.wikipedia.org/wiki/CMYK) i inne?
            -   Jak losować liczby?
            -   Jak zmieniać kolor tła form-a?
            -   Jak wykonywać fragment kodu w zapętleniu co określony czas?
        -   Podpowiedz:
            -   Random r = new Random();
            -   this.BackColor = Color.FromArgb(r,g,b);
                gdzie r,g,b to liczby z przedziału od 0-255
            -   Timer - element z toolboxa
    
    7.  [X] No weź idź sobie
        -   Label z napisem "obowiązki" który idzie w twoja stronę
        -   Problem:
            -   Jak wykryć pozycję kursora?
            -   Jak wykonywać kod w pętli co określony czas?
        -   Podpowiedz:
            -   this.PointToClient(Cursor.Position).X
                this.PointToClient(Cursor.Position).Y
            -   ToolBox -> Timer
    
    8.  [X] Szyfr Cezara
        -   Podajemy wiadomość, liczbę przesunięć oraz 
            lewo/prawo a zwraca nam zaszyfrowaną wiadomość.
        -   Problem:
            -   Na jakiej zasadzie działa szyfr Cezara?
        -   Podpowiedz:
            -   Wszystko przesunięte o n liter w lewo/prawo
            -   int a = (int)'a';
            -   char b = (char)98;
            -   przyda sie reszta z dzielenia (mod) %
    
    9.  [ ] Uwaga skacze!
        -   Zasymuluj układ spadku swobodnego.
            Zrob button, usuń z niego napis i po kliknieciu button ma zacząć spacać spadkiem swodobnym.
        -   Problem: 
            -   Jak to jest że coś spada?
        -   Podpowiedz:
            -   v[prektosc] = g[grawitacja]\*t[czas]
            -   button odpala timer timer1.start();
            -   v = g \* t/1000;

3.  [ ] HARD MODE <code>[0/3]</code>
    1.  [ ] Rozwiązywanie układu równań za pomocą eliminacji Gaussa
        -   Posiadając n niewiadomych oraz n równań rozwiąż ukłąd równań.
    
    2.  [ ] [Arkanoid](http://www.victorygames.pl/screeny/gry/duze/5178.jpg)
        -   Stworzyć grę na podobę Arkanoid
    
    3.  [ ] [Roślinożercy i mięsożercy](https://github.com/Hefaj/portfolio/tree/master/Python/simulation) 
        -   Niech x i y będą liczebnościami roślinożerców i polujących 
            na nie drapieżników na jakimś zamkniętym obszarze. 
            Prędkości zmian obu populacji dane są równaniami 
            Lotki-Volterry:
            
            dx/dt = rx\*x
            dy/dt = ry\*y
            
            gdzie rx to rozrodczość populacji roślinożerców dana 
            wzorem rx = a - b\*x - c\*y,  na sukces rozrodczy ujemnie 
            wpływa liczebność własnej populacji (konkurencja o kryjówki, 
            miejsca rozrodu itp) jak i liczebność drapieżników. 
            Z kolei rozrodczość drapieżników dana jest 
            wzorem ry = -d +e\*x-f\*y - wpływa na nią pozytywnie liczbność 
            potencjalnych ofiar, a negatywnie zagęszczenie
            własnej populacji.
            
            Zasymuluj dynamikę układu dwóch gatunków dla 
            a=5, b=0.005, c=0.2, d=1, e=0.03, f=0.01 [1/rok] 
            w pierwszych 10 latach oddziaływania populacji. 
            W chwili początkowej liczebności gatunków wynoszą 
            x0 = 60, y0 = 20.

4.  [X] Przemyślenia
    -   c      - system operacyjny, mikrokontrolery
    -   c++    - silnik gry, mikrokontrolery, UNREAL ENGINE
    -   c#     - $$$, UNITY
    -   java   - aplikacje mobline, podobnie zastosowanie co w c#
    -   Python - obliczenia fizyczne, matematyczne, AI
    -   R      - statystyka
    -   PHP    - webowe klient - serwer
    -   JS     - webowe klient, UNITY
    -   Oczwiście w JS czy w R też można robic AI, chodzi mi o to
        że częsciej używa się w tym Python albo c++.

