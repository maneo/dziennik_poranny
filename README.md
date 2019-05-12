# dziennik_poranny
Dziennik Poranny był wydawany w Poznaniu między 1935 a 1939 rokiem. 

Skany Dziennika dostępne są na stronach Wielkopolskiej Biblioteki Cyfrowej: http://www.wbc.poznan.pl/publication/29239. 

Plik streets.csv zawierają informacje na temat ulic o których wzmianki znalazłem w konkretnych numerach Dziennika Porannego. 

```
oai_id;street_name;longitude;latitude;order_of_page;original_filename
oai:www.wbc.poznan.pl:46605;bacha;16.9160578;52.3915747;first_page;0022.djvu
oai:www.wbc.poznan.pl:46605;fredry;16.9177031;52.4096504;first_page;0022.djvu
```

* oai_id - identyfikator OAI wskazujący na publikacje w WBC
* street_name - nazwa ulicy 
* longitude + latitude - współrzędne ulicy
* order_of_page - czy strona na której znaleziono nazwę ulicy to pierwsza, ostatnia czy inna strona
* original_filename - nazwa pliku

Znalezione nazwy to wynik działania skryptu, może zawierać błędy.
