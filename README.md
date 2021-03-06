
# Table of Contents

1.  [Konsola](#org0000c34)
2.  [WinForms](#org349102d)
3.  [Szlifowanie skila](#org8d35dc7)
4.  [HARD MODE](#org3643de1)
5.  [Konkretne zadania.](#orgd6df5a1)


<a id="org0000c34"></a>

# Konsola

-   Zadania <code>[8/14]</code>
    1.  [ ] Palindrom
        -   Sprawdzić czy podany napis jest palindromem.
        -   Problem:
            -   Co to palindrom?
        -   Podpowiedz:
            -   Słowo, które czyta się tak samo od przodu i od tyłu np. kajak.
    
    2.  [X] Tabliczka mnożenia
        -   Wyświetlić tabliczke mnożenia za pomocą for, while oraz do While
        -   Problem:
            -   Po co tyle pętli?
            -   Jak używać tych pętli?
        -   Podpowiedz:
            -   for(iterator; warunek; inkrementacja) {}
            -   while (warunek) {}
            -   do {} while (warunek);
    
    3.  [X] Bip bip
        -   Zrobić bip za pomocą pętli while
        -   Problem?
            -   To co ma byc Bip bip?!
            -   Jak się robi bip?
        -   Podpowiedz:
            -   Console.Beep(czestotliwosc[Hz], czas[ms] );
            -   czestotliwosc = <37-32767>, czas 100ms
    
    4.  [X] Algorytm Euklidesa (NWD)
        -   Policzyć najwiekszy wspólny dzielnik dwóch liczb
        -   Problem:
            -   Jak wygląda algorytm NWD?
        -   Podpowiedz:
            1.  oblicz c jako resztę z dzielenia a przez b
            2.  zastąp a liczbą b, następnie b liczbą c
            3.  jeżeli wartość b wynosi 0, to a jest szukaną wartością NWD, 
                w przeciwnym wypadku przejdź do kroku 1
    
    5.  [X] Silnia
        -   Obliczyć silnie z liczny n.
        -   Problem:
            -   Jak się liczy silnie?
        -   Podpowiedz:
            -   !n = 1 \* 2 \* .. \* n
    
    6.  [X] Lotto
        -   Generowanie 6-ciu liczb z zakresu 1-49 bez powtórzeń.
        -   Problem:
            -   Jak losować bez powtórzeń?
        -   Podpowiedz:
            -   Tablica z liczbami 1,2,&#x2026;, 49 
                wymieszać i wyświetlić pierwsze 6
            -   int tablica = new int[49];
            -   optymalne rozwiązanie
    
    7.  [X] Liczba Eulera
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
    
    8.  [ ] Liczby pierwsze
        -   Wyświetlić wszystkie liczby pierwsze z przedziału od 2 do n.
        -   Problem:
            -   Co to jest liczba pierwsza?
            -   Jak sprawdzić czy liczba jest pierwsza?
        -   Podpowiedz:
            -   Znając liczbę pierwszą można wykluczyć jej wielokrotności.
    
    9.  [X] Rozpisanie liczby
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
    
    10. [ ] Pochodna w punkcie
        -   Mając funkcje f(x) podać wartość pochodnej tej funkcji
            w wyznaczonym punkcie.
        -   Problem:
            -   Co to jest pochodna?
            -   Jak zakodować wzór pochodnej?
        -   Podpowiedz:
            -   Wyprowadzenie wzoru na pochodną ze wzoru Taylora
    
    11. [X] Wyświetlanie choinki
        -   Za pomocą pętli wyświetlić trójkąt prostokątny z '\*' 
            dla danego n.
        -   Problem:
            -   BRAK
        -   Podpowiedz:
            -   np. n = 3
                -   .
                -   ..
                -   &#x2026;
    
    12. [ ] Sortowanie tablicy liczb całkowitych
        -   Posortowanie rosnąco tablice liczb całkowitych.
        -   Problem:
            -   Jak wydajnie poukładać cyfry na swoich miejscach
        -   Podpowiedz:
            -   Array.Sort(array);
    
    13. [ ] Złota liczba
        -   Podaj wartość złotej liczby.
        -   Problem:
            -   Co to jest złota liczba?
        -   Podpowiedz:
               1+1
              1+2
             2+3
            3+5
    
    14. [ ] Miejsce zerowe funkcji
        -   Mając funkcje f(x) chcemy znaleźć miejsce zerowe z przedziału <a,b>
        -   Problem:
            -   Jak?
        -   Podpowiedz:
            -   Metoda bisekcji
    
    15. [ ] Całka Riemanna (oznaczona)
        -   Mając f(x) policzyć całkę Riemanna na przedziale <a,b>.
        -   Problem:
            -   Na czym polega całkowanie?
        -   Podpowiedz:
            -   Metoda Trapezów
                Pole trapezu => (a+b)\*h/2
                Sprawdzić całkowanie dla f(x)=2x xe0..1


<a id="org349102d"></a>

# WinForms

-   Zadania <code>[7/11]</code>
    1.  [ ] Puchnie jak balon
        -   Guzik który rośnie w trakcie trzymania myszy na nim.
            Kiedy się go kliknie, resetuje się do normalnych rozmiarów.
        -   Podpowiedz:
            -   Toolbox
            -   Właściwości button-a.
            -   event -> MouseMove()
    
    2.  [ ] Muzyczko graj!
        -   Zrobić 5 guzików, każdy z nich wywołuje inny dzwięk.
        -   Problem:
            -   Jak wywołać dzwięk?
        -   Podpowiedz:
            -   Console.Beep(c,t);
                c - czestotliwosc <37-32767>
                t - czas [ms]
    
    3.  [ ] Sterowanie klawiszami
        -   Poruszaj textBox-em za pomocą klaiwszy, wartość textBox-a to prętkość poruszania się.
        -   Podpowiedz:
            -   ToolBox -> textbox
    
    4.  [X] Napis 
        -   Program który pozwala wybrać z listy wielkość napisu.
            I zmienia rozmiar napisu na jaki wybraliśmy.
        -   Problem:
            -   Jak zmieniać rozmiar napisu?
            -   Jak zrobić rozwijalną liste?
        -   Podpowiedz:
            -   label.Font = new Font("Arial", 20); 20 <- rozmiar
            -   ToolBox - > ComboBox
            -   ComboBox -> events -> SelectedIndexChanged
    
    5.  [X] Pora roku
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
    
    6.  [X] Liczba parzysta
        -   Program sprawdzający czy wpisana liczba jest liczbą parzystką.
        -   Problem:
            -   Kiedy liczba jest parzysta?
        -   Podpowiedz:
            -   Liczba jest parzysta jeżeli reszta z dzielenia przez 2 jest równa 0.
    
    7.  [X] Uciekający textbox
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
    
    8.  [X] Dynamiczna zmiana koloru checkbox-a
        -   Wpisując w textbox-a ma się znieniać kolor tła.
        -   Problem:
            -   Jak zmieniać kolor tła?
        -   Podpowiedz:
            -   this.BackColor = Color.FromArgb(r,g,b);
    
    9.  [ ] Oczopląs
        -   Migający form na losowe kolory
        -   Problem:
            -   W jaki sposób komputer "rozumie" kolory, jak się je przedstawia, [RGB](https://pl.wikipedia.org/wiki/RGB), [CMYK](https://pl.wikipedia.org/wiki/CMYK) i inne?
            -   Jak losować liczby?
            -   Jak zmieniać kolor tła form-a?
            -   Jak wykonywć fragment kodu co określony czas?
        -   Podpowiedz:
            -   Random r = new Random();
            -   this.BackColor = Color.FromArgb(r,g,b);
                gdzie r,g,b to liczby z przedziału od 0-255
            -   Timer - element z toolboxa
    
    10. [X] No weź idź sobie
        -   Label z napisem "obowiązki" który idzie w twoja stronę
        -   Problem:
            -   Jak wykryć pozycję kursora?
            -   Jak wykonywać kod w pętli co określony czas?
        -   Podpowiedz:
            -   this.PointToClient(Cursor.Position).X
                this.PointToClient(Cursor.Position).Y
            -   ToolBox -> Timer
    
    11. [X] Szyfr Cezara
        -   Podajemy wiadomość, liczbę przesunięć oraz 
            lewo/prawo a zwraca nam zaszyfrowaną wiadomość.
        -   Problem:
            -   Na jakiej zasadzie działa szyfr Cezara?
        -   Podpowiedz:
            -   Wszystko przesunięte o n liter w lewo/prawo
            -   int a = (int)'a';
            -   char b = (char)98;
            -   przyda sie reszta z dzielenia (mod) %
            -   (char)((((int)litera-97)+n)%25)+97;
    
    12. [ ] Uwaga skacze!
        -   Zasymuluj układ spadku swobodnego.
            Zrob button, usuń z niego napis i po kliknieciu button ma zacząć spacać spadkiem swodobnym.
        -   Problem: 
            -   Jak to jest że coś spada?
        -   Podpowiedz:
            -   v[prektosc] = g[grawitacja]\*t[czas]
            -   button odpala timer timer1.start();
            -   v = g \* t/1000;


<a id="org8d35dc7"></a>

# Szlifowanie skila

-   Zadania <code>[0/3]</code>
    1.  [ ] Choinka<sub>2</sub>
        -   Dla podanego n wyświetlić        
               o    | 1
              o o   | 2
             o o o  | 3 
            o o o o | n
    
    2.  [ ] Szyfr cezara dla całych zdań
        -   Podajemy całe zdanie a program szyfruje metodą szyfru Cezara.
    
    3.  [ ] Liczba doskonała
        -   Sprawdzić czy podana liczba jest liczbą doskonałą.
        -   Problem:
            -   Co to jest liczba doskonała?
            -   Jak sprawdzić czy podana liczba jest liczbą doskonałą?
        -   Podpowiedz:
            -   dzielniki liczby 6 to 1, 2 i 3 czyli 1+2+3 = 6, 
                liczba 6 jest liczbą doskonałą (28, 496 tez)
            -   każda liczba dzieli się przez 1
            -   znajdź wszystkie dzielniki podanej liczby i zapisuj je do tablicy


<a id="org3643de1"></a>

# HARD MODE

-   Zadania <code>[0/5]</code>
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
    
    4.  [ ] Perceptron
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
    
    5.  [ ] Uczenie perceptronu
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


<a id="orgd6df5a1"></a>

# Konkretne zadania.

-   [Konkretne zadania, powodzenia.](https://github.com/Hefaj/Giganci/blob/master/img/more.png)


