# IMS Ecosystem - przykład dokumentu

## High Level Design

Data utworzenia: 29.03.2019

Data ostatniej modyfikacji: 29.03.2019

Wersja: 1.00

Status: do akceptacji


## Spis treści

[1. Historia dokumentu](#_historia_dokumentu)

[2. Przykłady nagłówków](#_przyklady_naglowkow)

[3. Przykład użycia tabeli](#_tab_zwykla)

[4. Przykład użycia tabeli z łączonymi komórkami w wersach](#_przyklad_uzycia_z_laczonymi_komorkami_w_wersach)

[5. Przykład użycia tabeli z łączonymi komórkami w wersach_i_kolumnach](#_tab_z_lacz_kom)

[6. Przykład użycia tabeli z szerokimi komórkami](#_tab_z_szer_kom)

[7. Blok tekstu - przykład](#_blok_tekstu)

[8. Umieszczenie kodu](#_kod)

[9. Przykład listy numerowanej](#_lista_numerowana)

[10. Przykład listy wypunktowanej z wcięciami](#_lista_wypunktowana)

[11. Formatowanie tekstu](#_formatowanie_tekstu)

[12. Użycie linku](#_link)

[13. Wstawienie rysunku](#_rysunek)

[14. Wstawienie dokumentu](#_dokument)

[15. Przykład komentarza](#_komentarz)



## Rysunki

[ rysunek1 ]: gfx/rysunek1.png	"Rysunek 1"
[rysunek2]: gfx/rysunek2.png	"Rysunek 2"
[rysunek3]:gfx/rysunek3.png

1. [Rysunek 1](#rysunek-1)

2. [Rysunek 2](#rysunek-2)

3. [Rysunek 2](#rysunek-3)
4. [My great heading](#1234)

   

## Tabele

1. [Tabela zwykła](#tabela-zwykła)
2. [Tabela z łączonymi komórkami](#tabela-z-łączonymi-komorkami)
3. [Tabela z szerokimi komórkami](#tabela-z-szerokimi-komórkami)



### My Great Heading {#1234}



<a id="_historia_dokumentu"> </a>

## Historia dokumentu

| LP      | Autor | Data | Zakres |
| ----------- | ----------- | ------------- | ---------- |
| 1 | Vimana Solutions | 01.04.2019 | Utworzenie dokumentu|

<a id="_przyklady_naglowkow"> </a>

## Przykłady nagłówków
# Nagłówek stopnia 1
## Nagłówek stopnia 2
### Nagłówek stopnia 3
#### Nagłówek stopnia 4
<a id="_przyklad_uzycia_tabeli"> </a>

## Przykład użycia tabel
<a id="_tab_zwykla"> </a>

Przykład użycia tabeli zwykłej bez stosowania html-a

#### Tabela Zwykła

| Kolumna 1 | Kolumna 2 | Kolumna 3 | Kolumna 4 | Kolumna 5 |
|---|---|---|---|---|
|kolumna 1, wiersz 1 | k2, w1 | k3, w1 | k4, w1 | k5, w1 |
|kolumna 1, wiersz 2 | k2, w2 | k3, w2 | k4, w2 | k5, w2 |
|kolumna 1, wiersz 2 | k2, w2 | k3, w2 | k4, w2 | k5, w2 |

<a id="_przyklad_uzycia_z_laczonymi_komorkami_w_wersach_i_kolumnach"> </a>

Przykład użycia tabeli z łączonymi komórkami zakodowanej w html-u

<a id="_tab_z_lacz_kom"> </a>

#### Tabela Z Łączonymi Komórkami

<table>
    <thead>
        <tr>
            <th>Kolumna 1</th>
            <th>Kolumna 2</th>
            <th>Kolumna 3</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan=4>K1, w1, 2, 3 i 4<br/>Nowa linia w kolumnie</td>
            <td rowspan=2>K2, w1 i 2</td>
            <td>K3, w 1</td>
        </tr>
        <tr>
            <td>K3, w2</td>
        </tr>
        <tr>
            <td rowspan=2>K2, w3 i 4</td>
            <td>K3, w3</td>
        </tr>
        <tr>
            <td>K3, w4</td>
        </tr>
    </tbody>
</table>
<a id="_przyklad_uzycia_z_szerokimi_komorkami"> </a>

<a id="_tab_z_szer_kom"> </a>Przykład użycia tabeli z szerokimi kolumnami (tworzy się pod spodem pasek poziomego przewijania)

#### Tabela Z Szerokimi Komórkami

| Kolumna 1 | Kolumna 2 | Kolumna 3 | Kolumna 4  |
|---|---|---|---|
| *Pierwsza_szeroka_kolumna* | Druga_szeroka_kolumna | Trzecia_jeszcze_szersza_kolumna | Czwarta_szeroka_kolumna |

<a id="_blok_tekstu"> </a>

## Blok tekstu - przykład
> "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Proin nibh augue, suscipit a, scelerisque sed, lacinia in, mi. Cras vel lorem. Etiam pellentesque aliquet tellus. Phasellus pharetra nulla ac diam. Quisque semper justo at risus. Donec venenatis, turpis vel hendrerit interdum, dui ligula ultricies purus, sed posuere libero dui id orci. Nam congue, pede vitae dapibus aliquet, elit magna vulputate arcu, vel tempus metus leo non est. Etiam sit amet lectus quis est congue mollis. Phasellus congue lacus eget neque. Phasellus ornare, ante vitae consectetuer consequat, purus sapien ultricies dolor, et mollis pede metus eget nisi. Praesent sodales velit quis augue. Cras suscipit, urna at aliquam rhoncus, urna quam viverra nisi, in interdum massa nibh nec erat."

<a id="_kod"> </a>

## Umieszczenie kodu

```mysql
mysql> desc Bookings;

**+---------------+-------------+------+-----+---------+----------------+**

**| Field | Type | Null | Key | Default | Extra |**

**+---------------+-------------+------+-----+---------+----------------+**

**| bk_id | int(11) | NO | PRI | NULL | auto_increment |**

**| bk_num_a | varchar(20) | YES | | NULL | |**

**| bk_starttime | bigint(20) | NO | MUL | NULL | |**

**| bk_endtime | bigint(20) | NO | MUL | NULL | |**

**| bk_maxmembers | int(11) | NO | | 5 | |**

**+---------------+-------------+------+-----+---------+----------------+**
```
<a id="_lista_numerowana"> </a>

## Przykład listy numerowanej
1. Punkt pierwszy, punkt pierwszy, punkt pierwszy,punkt pierwszy,punkt pierwszy,punkt pierwszy,punkt pierwszy,punkt pierwszy,punkt pierwszy,punkt pierwszy
   * podpunkt
   * kolejny podpunkt
2. Punkt drugi
3. Punkt trzeci

<a id="_lista_wypunktowana"> </a>

## Przykład listy wypunktowanej z wcięciami
Lista wypunktowana:
* punt pierwszy
* punkt drugi
* punkt trzeci
  * podpunkt
  * podpunkt
    *  zagnieżdżenie podpunktu
    *  kolejne zagnieżdżenie podpunktu
* punkt czwarty

<a id="_formatowanie_tekstu"> </a>

## Formatowanie tekstu
**tekst pogrubiony**

*tekst pochylony*

`tekst zaznaczony`

<a id="_link"> </a>

## Użycie linku:
[Przykład linku do zasobów sieci](http://google.pl)

<a id="_rysunek1"> </a>

## Wstawienie rysunku 
### Rysunek 1
<a id="_rysunek1"> </a>
![Rysunek 1][rysunek1]

### Rysunek 2
![Rysunek 2][rysunek2]

## Dołączenie dokumentu
<a id="_dokument"> </a>
Tutaj przykład dokumentu dołączonego
[czytaj](included.md)

## Komentarz

[//]: # "(Popularny, działający niezależnie od platform komentarz)"