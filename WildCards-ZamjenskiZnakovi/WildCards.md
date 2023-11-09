# WildCards - zamjenski znakovi
1. Što su zamjenski znakovi.
2. Kada i gdje se mogu koristiti.
3. Različite vrste zamjenskih znakova.
4. Kako koristiti zamjenske znakove s raznim naredbama.

## 1. Što su zamjenski znakovi.
Znak ili niz znakova koji se koristi za uzorak podudaranje.
Proširuje uzorak zamjenskog znaka u popis datoteka i/ili direktorija.

2. Kada i gdje se mogu koristiti.
Zamjenski znakovi mogu se koristiti s većinom naredbi
-	ls
-	rm
-	cp
-	…….

3. Različite vrste zamjenskih znakova.
* - odgovara nula ili više znakova.
    -	*.txt
    -	a*
    -	a*.txt
? - odgovara točno jednom znaku.
    -	?.txt
    -	a?
    -	a?.txt
[] - Klasa znakova.
     -	Odgovara bilo kojem od znakova uključenih između zagrade. Odgovara točno jednom znaku.
        * [aeiou]
        * ca[nt]*
          * can
          * cat
          * candy
          * catch
[!] - Odgovara bilo kojem od znakova koji NISU uključeni između zagrada. Odgovara točno jednom znaku.
      -	[!aeiou]*
        -	Baseball
        -	cricet
Koristite dva znaka odvojena crticom za stvaranje raspona u klasi znakova.
- [a-g]*
   - Podudara se sa svim datotekama koje počinju s a, b, c, d, e, f ili g.
- [3-6]*
   - Odgovara svim datotekama koje počinju s 3, 4, 5 ili 6.
Unaprijed definirane klase:
- [[:alpha:]] – slova, mala i velika
- [[:alnum:]] - alfanumerički znakovi, mala i velika slova
- [[:digit:]] – brojevi (i decimalni) od 0 do 9
- [[:lower:]] – mala slova
- [[:space:]] – razmak, tab, novi red …..
- [[:upper:]] – velika slova

Što ako želimo „pogoditi“ zamjenski znak?
Onda biste trebali „izbjeći“ taj znak s '\' prije tog znaka.
Preporuka: “Ako želiš sebi olakšati život, ne nazivajte svoje datoteke s upitnicima i zvjezdicama!“
Ukoliko hoćemo „pogoditi“ sve datoteke koje završavaju s upitnikom:
- *\?
  - done?
