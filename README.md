# Task 1
### Subtask 1
9/10

***
### Subtask 2
<i>done</i> 

***
### Subtask 3
Jestem Ewa, mam 33 lata i prawie 10 lat doświadczenia w szołbiznesie (iwęty, koncerty, reklama). 
Mam dosyć bycia odpowiedzialną za wszystkich dających ciała, więc chcę robić coś co zależy tylko ode mnie.
<BR>
Dlatego się przebranżawiam. A że kierownik produkcji musi myśleć do przodu, to robię sobie dwie nowe nogi:
QA i Scrum Master.
<BR>
Obecnie jestem na bezpłatnym dla obu stron stażu/kursie na QA. Może uda mi się zaczepić w tej firmie, a może nie, więc 
zwiększam swoje szanse na znalazienie pierwszej popracy przez uczestnictwo w challengu. 
Chcę sprawdzić w innym środowisku czego mnie nauczyli na tym kursostażu.

***
### Subtask 4
<i>Jest to aplikacja dla skautów piłki nożnej, która umożliwia przeglądanie wskaźników, umiejętności i pozycje zawodników.</i>
<BR><BR>  
 ***
<i>Funkcjonalności znajdują się w aplikacji? Do czego służą. Czy są intuicyjne, czy może byś coś zmienił_a? </i>
* dodanie nowego gracza
* dodanie nowego meczu
* dodanie raportu z meczu
* spis graczy
* możliwość wydrukowania listy i wygenerowania pliku .csv
***
<i>Oceń interfejs aplikacji (wygląd) – czy Ci się podoba, czy nie?</i>
Interfejs jest prosty, ubogi, ale nie uważam tego za minus - na początek wystarczający. Dodałabym elementy typu logo, informację o zalogowanym użytkowniku 
***
   
<i>Czy aplikacja jest intuicyjna? (Intuicyjna, czyli np. nie masz problemu ze zrozumieniem, co należy kliknąć, żeby wejść do formularza dodawania nowego zawodnika piłki nożnej do systemu).</I>
No nie jest. Gdzie na pierwszy rzut oka mogę dodać mecz? Albo raport? A
***
   <i>Czy zauważasz jakieś błędy? Albo coś wydaje Ci się błędem? </i>
   No kilka się znajdzie ale spodziewam się, że będzie to następnym taskiem, to sobie zachowam :)
***
Tested on Brave.<BR><BR>

### dekompozycja:
* logowanie
    * login 
      * prawidłowy email (z dostępnej puli)
      * nieistniejący email
      * nie podawaj emaila
    * hasło
      * prawidłowe hasło
      * nieprawdiłowe hasło
      * nie wpisuj hasła
    * przypomnij hasło
      * podaj prawidłowy email 
      * podaj inny niż... email
      * nie podawaj emaila
      * podaj email z błędem (spacją, nieistniejący)
    * wybór języka
      * zmień język
   
* UWAGI:
1) "Scouts Panel" w pl i ang wersji, może panel scouta w pl?
2) po nieudanym logowaniu UI się rozjeżdża 
3) Przy wybranym j. polskim walidacja uzupełnionych pól jest w j. angielskim
4) Przypomnij hasło - brak walidacji czy podany email jest w bazie i czy jest sens wysyłać do niego przypomnienie maila
5) Przypomnij hasło też wysyła na brak maila, przycisk SEND robi się nieaktywny
   
 * main page
    * boczne menu
      * Strona główna
      * Gracze
      * wybór języka
      * Wyloguj
    * Linki pomocnicze
      * dodaj gracza
    * Aktywność
      * ostatnio stworzony gracz
      * ostatnio zaktualizowany gracz
      * ostatnio stworzony mecz
      * ostatnio zaktualizowany mecz
      * ostatnio zaktualizowany raport
      
* UWAGI:
1) wszystko działa z grubsza
2) nieintuicyjne, trzeba szukać i się zastanawiać co gdzie: gdzie jest dodanie meczu? Gdzie jest dodawanie raportu? IDK
      
      
 * dodaj gracza
    * boczne menu
      * Strona główna
      * Gracze
      * wybór języka
      * Wyloguj
    * cały formularz dodawania gracza 
     *brak '*' przy wymaganych uzupełnienia polach
      * e-mail
        * liczba znaków (n, n-1, n+1)
        * format maila - nie istniejące
        * mail ze spacją
      * imię
        * liczba znaków (n, n-1, n+1)
        * spacje
        * cyfry
        * znaki specjalne
      * naziwsko
        * liczba znaków (n, n-1, n+1)
        * spacje
        * cyfry
        * znaki specjalne
      * telefon
        * liczba znaków (n, n-1, n+1)
        * format zapisu numeru telefonu
        * spacje
        * litery
        * znaki specjalne
        * wartości ujemne
      * waga
        * liczba znaków (n, n-1, n+1)
        * format zapisu numeru telefonu
        * spacje
        * litery
        * znaki specjalne
        * wartości ujemne
      * wzrost
        * liczba znaków (n, n-1, n+1)
        * format zapisu numeru telefonu
        * spacje
        * litery
        * znaki specjalne
        * wartości ujemne
      * data
        * poprawne dane (przed datą uzupełnienia)
        * po dacie uzupełnienia
        * poprawne daty walidacja wieku
      * dominująca noga
        * dropdown menu
      * klub
        * liczba znaków (n, n-1, n+1)
      * poziom rozgrywek
        * liczba znaków (n, n-1, n+1)
      * główna pozycja
        * liczba znaków (n, n-1, n+1)
      * pozycja alternatywna
        * liczba znaków (n, n-1, n+1)
      * województwo
        * dropdown menu
      * osiągnięcia
        * liczba znaków (n, n-1, n+1)
      * dodaj język
        * click
         * języki
          * liczba znaków (n, n-1, n+1)
          * ikona śmietnika
      * łączy nas piłka, 90 minut, profil FB
        * liczba znaków (n, n-1, n+1)
        * format zapisu
      * dodaj link z YT
        * click
         * link do YT
          * liczba znaków (n, n-1, n+1)
          * ikona śmietnika     
* UWAGI:
1) Paskudny formularz
2) ostrzeżenie o brakach danych po kliknięciu "SUBMIT" "po kolei" a nie od razu hurtem, czego brakuje
3) ale po "CLEAR" już mamy wymagane poświetlone
   
   * ostatnio stworzony gracz i ostatnio zaktualizowany gracz
      * ten sam formularz co "dodaj gracza" patrz *90
 * UWAGI:
1) Dlaczego to jest ten sam formularz, który umożlwia edycję. Chcę zobaczyć ostatnio stworzonego/zaktualizowanego gracza a z poziomu oglądania chcę zdecydować o edycji

