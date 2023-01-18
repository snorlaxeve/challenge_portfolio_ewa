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
Tested on Brave.<BR><BR>

dekompozycja:
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
    * Aktywność
      
* UWAGI:
1) wszystko działa
2) po nieudanym logowaniu UI się rozjeżdża 
3) Przy wybranym j. polskim walidacja uzupełnionych pól jest w j. angielskim
4) Przypomnij hasło - brak walidacji czy podany email jest w bazie i czy jest sens wysyłać do niego przypomnienie maila
5) Przypomnij hasło też wysyła na brak maila, przycisk SEND robi się nieaktywny
