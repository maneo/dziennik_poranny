# dziennik_poranny
Dziennik Poranny był wydawany w Poznaniu w latach 1935 - 1939. 

Skany Dziennika dostępne są na stronach Wielkopolskiej Biblioteki Cyfrowej: http://www.wbc.poznan.pl/publication/29239. 

W tym repozytorium znajdziecie dodatkowe metadane opisujące kolejne wydania Dziennika Porannego. Dołożyłem wszelkich starań, aby zweryfikować opublikowane tutaj dodatkowe metadane, ale mogą one zawierać błędy.

Plik ```streets.csv``` zawierają informacje na temat ulic o których wzmianki znalazłem w konkretnych numerach Dziennika Porannego. 

```
id,oai_id,value,order,file,verified,entry_type,has_attach,display_name,link_to_content
10,oai:www.wbc.poznan.pl:46605,podgórna,last_page,0024.djvu,1,1,FALSE,ul. podgórna,https://www.wbc.poznan.pl/dlibra/publication/edition/46605
1001,oai:www.wbc.poznan.pl:46996,wolności,first_page,0675.djvu,5,1,FALSE,pl. wolności,https://www.wbc.poznan.pl/dlibra/publication/edition/46996
10013,oai:www.wbc.poznan.pl:47633,wielka,other_page,1218.djvu,5,1,FALSE,ul. wielka,https://www.wbc.poznan.pl/dlibra/publication/edition/47633
```

Pola ogólnego użytku:
* oai_id - identyfikator OAI wskazujący na publikacje w WBC
* value - nazwa rozpoznanej ulicy bez prefixu
* order - czy strona na której znaleziono nazwę ulicy to pierwsza, ostatnia czy inna strona (możliwe wartości: first_page, other_page, last_page)
* file - plik/strona na wewnątrz gazety
* display_name - nazwa rozpoznanej ulicy/placu/alei - w miarę możliwości używać tej nazwy
 

Pola techniczne systemu NEP:
* id - identyfikator zidentyfikowanego wpisu w systemi NEP
* verified - stan weryfikacji danego wpisu, wartości: 1 i 5 oznaczają 
* has_attach - informacja o tym czy z danym wpisem jest skojarzony załącznik graficzny 
* entry_type - typ wpisu, własność w systemi NEP


Plik ```add_metadata.csv``` zawiera dodatkowe metadane opisujące zawartość numerów, są to wszystkie informacje, które uznałem za wartościowe. 

```
id,oai_id,value,order,file,verified,entry_type,has_attach,link_to_content
13086,oai:www.wbc.poznan.pl:46605,niewolnica maharadży,other_page,0023.djvu,1,2,FALSE,https://www.wbc.poznan.pl/dlibra/publication/edition/46605
13087,oai:www.wbc.poznan.pl:46605,uśmiechnij się (rubryka),other_page,0021.djvu,1,2,FALSE,https://www.wbc.poznan.pl/dlibra/publication/edition/46605
13088,oai:www.wbc.poznan.pl:46605,dobre rady pani wandy (rubryka),other_page,0021.djvu,1,2,FALSE,https://www.wbc.poznan.pl/dlibra/publication/edition/46605
```

Pola ogólnego użytku:
* oai_id - identyfikator OAI wskazujący na publikacje w WBC
* value - nazwa rozpoznanej ulicy bez prefixu
* order - czy strona na której znaleziono nazwę ulicy to pierwsza, ostatnia czy inna strona (możliwe wartości: first_page, other_page, last_page)
* file - plik/strona na wewnątrz gazety

Pola techniczne systemu NEP:
* id - identyfikator zidentyfikowanego wpisu w systemi NEP
* verified - stan weryfikacji danego wpisu, wartości: 1 i 5 oznaczają 
* has_attach - informacja o tym czy z danym wpisem jest skojarzony załącznik graficzny 
* entry_type - typ wpisu, własność w systemi NEP

Oprócz tych dwóch plików publikuje również słownik ulic/placów/alei które istniały w Poznaniu w 1938, plik ```street_names_entities.v2.json``` zawiera również warianty zapisu, wersję z błędami zapisu.

```
 {
  "main_name": "27 grudnia",
  "variants": [
   "27—go grudnia"
  ],
  "misspellings": [
   "27 grnri",
   "2710 grudnia",
   "27 gruzini-l"
  ],
  "prefix": "ul.",
  "display_name": "ul. 27 grudnia"
 },

```

