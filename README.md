
# Table of Contents

1.  [Zadanka<code>[0/4]</code>](#org740a994)


<a id="org740a994"></a>

# TODO Zadanka<code>[0/4]</code>

1.  [-] Konsola <code>[2/14]</code>
    1.  [X] Silnia
        -   Obliczy� silnie z liczny n.
        -   Problem:
            -   Jak si� liczy silnie?
        -   Podpowiedz:
            -   !n = 1 \* 2 \* .. \* n
    
    2.  [ ] Lotto
        -   Generowanie 6-ciu liczb z zakresu 1-49 bez powt�rze�.
        -   Problem:
            -   Jak losowa� bez powt�rze�?
        -   Podpowiedz:
            -   Tablica z liczbami 1,2,&#x2026;, 49 
                wymiesza� i wy�wietli� pierwsze 6
            -   int tablica = new int[49];
            -   optymalne rozwi�zanie
    
    3.  [ ] Liczba Eulera
        -   Napisa� program licz�cy przybli�enie liczby Eulera
        -   Problem:
            -   Co to jest liczba Eulera, jak j� liczy�?
        -   Podpowiedz:
            -   e = sum(1/n!) czyli 1/0! + 1/1! + 1/2! + &#x2026;
            -   zrobi� z silni funkcje
            -   static int silnia(n){\`[liczenie]\`  return s}
        -   Rozwi�zanie:
            -   for(i=0;i<n;i++)
                s+=1f/silnia(n)
    
    4.  [ ] Liczby pierwsze
        -   Wy�wietli� wszystkie liczby pierwsze z przedzia�u od 2 do n.
        -   Problem:
            -   Co to jest liczba pierwsza?
            -   Jak sprawdzi� czy liczba jest pierwsza?
        -   Podpowiedz:
            -   Znaj�c liczb� pierwsz� mo�na wykluczy� jej wielokrotno�ci.
    
    5.  [ ] Rozpisanie liczby
        -   Podaj�c liczb�, ma zosta� ona wy�wietlona w postaci sumy liczb.
            1234 = 1000 + 200 + 30 + 4
        -   Problem:
            -   Jak przechwyci� pojedyncze cyfry?
        -   Podpowiedz:
            -   string to tablica char�w 
                string liczba = "1234";
                liczba[0] => "1";
            -   stringi mo�na skleja� za pomoc� znaku "+"
                "ala" + "ma" + "kota" => "alamakota"
    
    6.  [ ] Pochodna w punkcie
        -   Maj�c funkcje f(x) poda� warto�� pochodnej tej funkcji
            w wyznaczonym punkcie.
        -   Problem:
            -   Co to jest pochodna?
            -   Jak zakodowa� wz�r pochodnej?
        -   Podpowiedz:
            -   Wyprowadzenie wzoru na pochodn� ze wzoru Taylora
    
    7.  [X] Wy�wietlanie choinki
        -   Za pomoc� p�tli wy�wietli� tr�jk�t prostok�tny z '\*' 
            dla danego n.
        -   Problem:
            -   BRAK
        -   Podpowiedz:
            -   np. n = 3
                -   .
                -   ..
                -   &#x2026;
    
    8.  [ ] Sortowanie tablicy liczb ca�kowitych
        -   Posortowanie rosn�co tablice liczb ca�kowitych.
        -   Problem:
            -   Jak wydajnie pouk�ada� cyfry na swoich miejscach
        -   Podpowiedz:
            -   Array.Sort(array);
    
    9.  [ ] Liczba doskona�a
        -   Sprawdzi� czy podana liczba jest liczb� doskona��.
        -   Problem:
            -   Co to jest liczba doskona�a?
            -   Jak sprawdzi� czy podana liczba jest liczb� doskona��?
        -   Podpowiedz:
            -   dzielniki liczby 6 to 1, 2 i 3 czyli 1+2+3 = 6, 
                liczba 6 jest liczb� doskona�� (28, 496 tez)
            -   ka�da liczba dzieli si� przez 1
            -   znajd� wszystkie dzielniki podanej liczby i zapisuj je do tablicy
    
    10. [ ] Z�ota liczba
        -   Podaj warto�� z�otej liczby.
        -   Problem:
            -   Co to jest z�ota liczba?
        -   Podpowiedz:
               1+1
              1+2
             2+3
            3+5
    
    11. [ ] Miejsce zerowe funkcji
        -   Maj�c funkcje f(x) chcemy znale�� miejsce zerowe z przedzia�u <a,b>
        -   Problem:
            -   Jak?
        -   Podpowiedz:
            -   Metoda bisekcji
    
    12. [ ] Ca�ka Riemanna (oznaczona)
        -   Maj�c f(x) policzy� ca�k� Riemanna na przedziale <a,b>.
        -   Problem:
            -   Na czym polega ca�kowanie?
        -   Podpowiedz:
            -   Metoda Trapez�w
                Pole trapezu => (a+b)\*h/2
                Sprawdzi� ca�kowanie dla f(x)=2x xe0..1
    
    13. [ ] Perceptron
        -   Stworzy� perceptron 2 wej�cia 1 wyj�cie.
        -   Problem:
            -   Co to jest perceptron (neuron matematyczny).
        -   Podpowiedz:
            -   Algebra liniowa
                x <- wektor wej�ciowy
                w <- wektor wag
                Q <- Funkcja progowa unipolarna 
                     czyli 0 dla <0 i 1 dla >=0
                T <- Transponowanie
                
                    x1       w1
                x =     w =   
                    x2       w2
                
                y = Q( T(x)\*w )
                w <- losowe z przedzia�u (0,1)
    
    14. [ ] Uczenie perceptronu
        -   Stworzy� algorytm uczenia perceptrony
            Czyli modyfikacji wag (w) aby zwraca�o co chcemy
        -   Problem:
            -   W jaki spos�b modyfikowa� wagi?
        -   Podpowiedz:
            -   Maj�c wynik (y) dla wektora ucz�cego x, x={x1,x2}
                i oczekuj�c od perceptronu wyj�cia y' dla wektora x.
                
                Mo�emy sprawdzi� czy y'-y = 0
                je�eli tak to znaczy, �e perceptron
                zwraca poprawne warto�ci.
                
                Je�eli nie to modyfikujemy wagi
                w1 += (y'-y)\*

2.  [-] WinForms <code>[3/8]</code>
    1.  [ ] Napis 
        -   Program kt�ry pozwala wybra� z listy wielko�� napisu.
            I zmienia rozmiar napisu na jaki wybrali�my.
        -   Problem:
            -   Jak zmienia� rozmiar napisu?
            -   Jak zrobi� rozwijaln� liste?
        -   Podpowiedz:
            -   label.Font = new Font("Arial", 20); 20 <- rozmiar
            -   ToolBox - > ComboBox
            -   ComboBox -> events -> SelectedIndexChanged
    
    2.  [ ] Pora roku
        -   Podajemy numer miesi�ca a program m�wi jak to pora roku.
            Grudzie� (12) - Luty     (2)  - Zima
            Marzec   (3)  - Maj      (5)  - Wiosna
            Czerwiec (6)  - Sierpie� (8)  - Lato
            Wrzesie� (9)  - Listopad (11) - Jesie�
        -   Podpowiedz:
            -   switch (n)
                case 3:
                case 4:
                case 5:
                    Console.Write&#x2026;
                    break;
    
    3.  [X] Liczba parzysta
        -   Program sprawdzaj�cy czy wpisana liczba jest liczb� parzystk�.
        -   Problem:
            -   Kiedy liczba jest parzysta?
        -   Podpowiedz:
            -   Liczba jest parzysta je�eli reszta z dzielenia przez 2 jest r�wna 0.
    
    4.  [X] Uciekaj�cy textbox
        -   Po najechaniu mysz� textbox ucieka w inne 
            losowe miejsce w naszym oknie.
        -   Problem:
            -   Jaka funkcja jest wykonywana po najechaniu na element?
            -   Jak wylosowa� liczb� z odpowiedniego przedzia�u?
            -   Jak zmieni� z pozycji kodu pozycj� textboxa?
        -   Podpowiedz:
            -   Piorunek nad w�a�ciwo�ciami.
            -   Random r = new Random();
                r.Next(a,b);
            -   box.location = new Point(x,y);
    
    5.  [X] Dynamiczna zmiana koloru checkbox-a
        -   Wpisuj�c w textbox-a ma si� znienia� kolor t�a.
        -   Problem:
            -   Jak zmienia� kolor t�a?
        -   Podpowiedz:
            -   this.BackColor = Color.FromArgb(r,g,b);
    
    6.  [ ] Oczopl�s
        -   Migaj�cy form na losowe kolory
        -   Problem:
            -   W jaki spos�b komputer "rozumie" kolory, jak si� je przedstawia, [RGB](https://pl.wikipedia.org/wiki/RGB), [CMYK](https://pl.wikipedia.org/wiki/CMYK) i inne?
            -   Jak losowa� liczby?
            -   Jak zmienia� kolor t�a form-a?
            -   Jak wykonywa� fragment kodu w zap�tleniu co okre�lony czas?
        -   Podpowiedz:
            -   Random r = new Random();
            -   this.BackColor = Color.FromArgb(r,g,b);
                gdzie r,g,b to liczby z przedzia�u od 0-255
            -   Timer - element z toolboxa
    
    7.  [ ] No we� id� sobie
        -   Label z napisem "obowi�zki" kt�ry idzie w twoja stron�
        -   Problem:
            -   Jak wykry� pozycj� kursora?
            -   Jak wykonywa� kod w p�tli co okre�lony czas?
        -   Podpowiedz:
            -   this.PointToClient(Cursor.Position).X
                this.PointToClient(Cursor.Position).Y
            -   ToolBox -> Timer
    
    8.  [ ] Szyfr Cezara
        -   Podajemy wiadomo��, liczb� przesuni�� oraz 
            lewo/prawo a zwraca nam zaszyfrowan� wiadomo��.
        -   Problem:
            -   Na jakiej zasadzie dzia�a szyfr Cezara?
        -   Podpowiedz:
            -   Wszystko przesuni�te o n liter w lewo/prawo
            -   int a = (int)'a';
            -   char b = (char)98;
            -   przyda sie reszta z dzielenia (mod) %

3.  [ ] HARD MODE <code>[0/2]</code>
    1.  [ ] [Arkanoid](http://www.victorygames.pl/screeny/gry/duze/5178.jpg)
        -   Stworzy� gr� na podob� Arkanoid
    
    2.  [ ] [Ro�lino�ercy i mi�so�ercy](https://github.com/Hefaj/portfolio/tree/master/Python/simulation) 
        -   Niech x i y b�d� liczebno�ciami ro�lino�erc�w i poluj�cych 
            na nie drapie�nik�w na jakim� zamkni�tym obszarze. 
            Pr�dko�ci zmian obu populacji dane s� r�wnaniami 
            Lotki-Volterry:
            
            dx/dt = rx\*x
            dy/dt = ry\*y
            
            gdzie rx to rozrodczo�� populacji ro�lino�erc�w dana 
            wzorem rx = a - b\*x - c\*y,  na sukces rozrodczy ujemnie 
            wp�ywa liczebno�� w�asnej populacji (konkurencja o kryj�wki, 
            miejsca rozrodu itp) jak i liczebno�� drapie�nik�w. 
            Z kolei rozrodczo�� drapie�nik�w dana jest 
            wzorem ry = -d +e\*x-f\*y - wp�ywa na ni� pozytywnie liczbno�� 
            potencjalnych ofiar, a negatywnie zag�szczenie
            w�asnej populacji.
            
            Zasymuluj dynamik� uk�adu dw�ch gatunk�w dla 
            a=5, b=0.005, c=0.2, d=1, e=0.03, f=0.01 [1/rok] 
            w pierwszych 10 latach oddzia�ywania populacji. 
            W chwili pocz�tkowej liczebno�ci gatunk�w wynosz� 
            x0 = 60, y0 = 20.

4.  [ ] Przemy�lenia
    -   c      - system operacyjny, mikrokontrolery
    -   c++    - silnik gry, mikrokontrolery, UNREAL ENGINE
    -   c#     - $$$, UNITY
    -   java   - aplikacje mobline, podobnie zastosowanie co w c#
    -   Python - obliczenia fizyczne, matematyczne, AI
    -   R      - statystyka
    -   PHP    - webowe klient - serwer
    -   JS     - webowe klient, UNITY
    -   Oczwi�cie w JS czy w R te� mo�na robic AI, chodzi mi o to
        �e cz�sciej u�ywa si� w tym Python albo c++.

