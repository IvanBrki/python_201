# Tekst na računalu

Prije no što se bacimo na programiranje s tekstom, korisno je razumjeti
kako računalo barata tekstom jer se to razlikuje od teksta zapisanog na
papiru ili kakvoj drugoj materijalnoj podlozi.

## SOS

Kako bi u opasnosti pozvali u pomoć ako vikanje ne pomaže? Recimo da se
radi o brodolomcu na pustom otoku ili brodu u opasnosti. Međunarodni
signal za pomoć se odašilje tako tako što pošaljemo tri kratka impulsa
(na primjer tri kratka zvuka ili tri kratka bljeska džepnom lampom),
zatim tri duga impulsa pa opet tri kratka impulsa. Ovaj signal se naziva
SOS i međunarodno je priznat signal za poziv u pomoć koristeći se
**Morseovom abecedom**. Originalno je razvijen za potrebe brodova u
nevolji, a koristi se od početka 20-og stoljeća. SOS je s vremenom
postao dovoljno poznat da se kasnije počinje koristiti za potrebe
odašiljanja poziva svima koji su dovoljno blizu da ga prime, a i kao
motiv u popularnoj kulturi poput glazbe. Također, SOS nije kratica za
ništa specifično. Odabran je radi distinktivnosti signala čime se
garantira njegova iskoristivost, a time se i olakšalo prihvaćanje
signala kao međunarodnog standarda.

Ovdje nas ne zanima toliko signal SOS koliko Morseova abeceda.
Preciznije ju možemo zvati Morseov **kod**. Taj kod se sastoji od dva
elementa: impulsa i stanke. Impuls može biti kratki ili dugi. Dugi
impuls traje kao tri kratka impulsa. Stanka služi pravljenju razmaka
između riječi i rečenica. Impulsi se mogu poslati bilo čime što se dobro
prenosi na velike udaljenosti. Primjeri uključuju zvuk, svjetlo, strujne
impulse i radio valove. Zvuk i svjetlo je relativno lako proizvesti bez
napredne tehnologije, ali otežavaju standardizaciju i iskoristivost.
Strujni impulsi su sigurniji za prijenos u lošim uvjetima, odnosno kada
postoji buka u komunikacijskom kanalu (npr. zvuk se neće prenijeti u
bučnim situacijama, a svjetlo je uglavnom iskoristivo noću), ali oni
zahtijevaju provedenu žicu. Ova tehnologija postaje najiskoristivija s
radio valovima koji omogućuju bežičnu komunikaciju, a kasnije ju
zamjenjuje prijenos ljudskog glasa putem istog medija. Kod je originalno
razvijen za potrebe električnog telegrafa. Zanimljivo je i da je to
posve digitalna metoda komunikacije budući da je signal ili prisutan ili
nije i to bez obzirom kojom se metodom prenosi.

Ono što nam je ovdje zanimljivo je kako Morseov kod kodira znakove. SOS
se dakle sastoji od tri kratka, tri druga, tri kratka impulsa. Ovo bi
tekstom mogli zapisati kao (\...---\...). Slovo S je dakle kodirano kao
(\...), a slovo O kao (---). Svako slovo prima varijabilan broj impulsa.
Slovo koje se češće koristi u engleskome govoru je zakodirano s manjim
brojem znakova. Slovo E je tako jednostavno zakodirano s (.). e!

Važno je primijetiti da je Morseov kod posve odvojen od bilo kakve
tipografije, odnosno \"crteža slova\" i pozicioniranja teksta na
podlogu. Kada njime prenesemo slovo \"e\", to je točno to slovo, ali je
posve odvojeno od prikaza tog slova. Za komunicirati dodatne značajke
tog slova, poput fonta, podebljanja ili nakošenosti, potrebne su nam
dodatne informacije koje u ovom slučaju samo otežavali komunikaciju za
razliku od tiskanog teksta u kojemu je omogućuju i potencijalno
olakšavaju.

``` important
Digitalan tekst Pošaljite signal SOS lupkajući o stol. Upravo ste
prenijeli digitalni, ali ne i elektronički tekst. Kako nakositi ili
podebljati slova? Kako promijeniti font? Razmišljanjem o tim pitanjima
doći ćete do razumijevanja razlike digitalnog teksta od teksta kakvim ga
poznajete s papira, pergamene, papirusa ili zida pećine. Takav tekst je
zapisan prikazom, a digitalan tekst se prenosi kodom koji nema nikakve
veze s prikazom teksta za potrebe njegova prenošenja.
```

## Kodiranje teksta

Napomenuli smo da SOS kodiramo Morseovim kodom. U ovom smislu, \"kod\"
je sustav pravila za konverziju informacija iz jednog oblika u drugi za
potrebe komunikacije. U ovom značenju \"kodiranje\" možemo shvatiti kao
\"šifriranje\", ali važno je zapamtiti da se u ovom tekstu riječ \"kôd\"
uglavnom koristi kako bi označila \"programski kôd\" što je drugo
značenje te riječi. Iako konceptu \"kodiranog teksta\", kao i riječi
\"šifra\", često pridodajemo koncept tajnosti, kodirani tekst vrlo često
nije tajan. Dapače, kako bi bio široko korišten, taj sustav pravila mora
biti javno dostupan i standardiziran. U ovom smislu \"kodirana
komunikacija\" se najčešće provodi između ljudi i strojeva, odnosno
informacije kodiramo kako bismo mogli koristiti strojeve za prijenos
istih. Prijevod slova engleske abecede i brojeva na Morseov kod kao i
pravila prijenosa su vidljiva na sljedećoj slici. Primijetite da točna
dužina impulsa nije propisana, samo odnos između kratkog i dugog
signala. U načelu čim brže možemo poslati dugi signal, tim bolje sve dok
se može dekodirati.

Prijevod teksta u neki kod nazivamo **kodiranje** (eng. *encoding*).
Prijevod iz koda u tekst nazivamo **dekodiranje** (eng. *decoding*). Kad
odvedemo ovu ideju dovoljno daleko dolazimo i do ljudskog jezika.

Dapače, zašto tekst zovemo \"t e k s t\"? Ta riječ ima svoju etimologiju
i potiče od latinskog *textus* što znači \"satkan\", odnosno koji je
nastao tkanjem. Radi se dakle o prenesenom značenju za potrebe
suvremenijeg koncepta ili korištenja, ali kad bi razmišljali o jeziku do
samih početaka vidjeli bi da je sam ljudski jezik na neki način kôd: to
je standardizirani sustav kodiranja stvari i koncepata radi prenošenja
informacija.

Ipak, ovaj tekst nećemo širiti do problema jezika već ćemo se fokusirati
na stroj koji nam je najvažniji za potrebe ovog gradiva: suvremeno
računalo. To je elektroničko digitalno računalo pa je glavni oblik
kodiranja teksta koji nas ovdje interesira zapisivanje teksta putem
binarnog koda, odnosno putem nula i jedinica jer je to sve što možemo
pohraniti u računalnu memoriju. Pojednostavljeno rečeno: struje ili ima
ili nema i to je upravo što nula i jedan u ovom kontekstu znače.

## Tekst i računalo

Tekst na računalu je neprekinuti niz znakova. Za razliku od Morseovog
načina kodiranja, ne postoji \"praznina\". Svaka promjena u tekstu je
znak. Razmak je znak. Prelazak u novi redak je znak. Sav ostali \"bijeli
prostor\" je znak. Velika i mala slova su različiti znakovi. Kada kažemo
\"običan tekst\" (eng. *plain text*) referiramo se samo na
reprezentaciju znakova u računalnoj memoriji bez ikakvih informacija o
tipografiji, odnosno o obliku slova (tj. fontu), o razmaku između slova,
riječi i redaka, o naslovima, paragrafima i razmaku među njima i bez
ikakvog koncepta \"stranice\" poput margina, orijentacije i sličnog.
Običan tekst jednostavno ne barata tim konceptima već se samo sastoji od
\"šifri\" za znakove u memoriji računala. Kako bismo zapisali spomenuto
potrebno nam je još teksta koji opisuje drugi tekst i govori stvari
poput \"ovaj izraz je naslov\", \"ovaj izraz je podebljan\", \"ovaj
izraz je uži od ostatka teksta i treba ga prikazati drugim fontom\".
Ovaj koncept nazivamo \"označavanje teksta\", a o tome ćemo nešto
detaljnije kasnije.

``` important
Zapis i prikaz računalnog teksta Računalni tekst je zapisan kodom, a
prikaz mu se dodjeljuje pravilima. Kada gledamo prikaz običnog teksta na
ekranu, računalo koristi dodatna formalna pravila kako bi svakom znaku
dodijelilo vizualni izričaj.
```

Šifra za jedan znak je dakle niz nula i jedinica u memoriji od kojih
određen broj predstavlja neki znak, na primjer slovo \"a\". Za razliku
od zida pećine ili papira (na koje slova \"crtamo\"), sam prikaz slova
\"a\" je nevezan za memorijski zapis ovog slova već je to druga razina
kad ovoj šifri dodijelimo neki proizvoljno odabran font. To slovo u
memoriji dakle nema niti veličinu znaka niti podržava koncepte kao što
su podebljanost ili nakošenost. To je jednostavno šifra za slovo \"a\",
a najčešće korištena šifra za to slovo je 01100001. U ovom smislu, nula
i jedinica su znamenke binarnog brojevnog sustava i individualnu nulu
ili jedinicu nazivamo bit. Osam bitova nazivamo bajt.

### ASCII

Tekst na računalu je dakle jedan neprekinuti niz znakova od kojih je
svaki kodiran (i.e. šifriran) s određenim brojem bitova. Kada bi znak
kodirali s jednim bitom podržavali bi samo dva znaka koja bi odgovarala
kodovima 0 i 1. Dva bita podržavaju četiri znaka. Broj različitih
kombinacija (*r*) od određenog broja znakova (*n*) je jednostavno $n^r$.
Šest bitova, šest nula ili jedinica, podržava dakle 64 različite
kombinacije putem kojih možemo zakodirati 64 različitih znakova, sedam
bitova 128, a osam bitova 256. Početak kodiranja znakova za potrebe
računala se temeljio na telegrafskim šiframa i idejama. Tako 1963
nastaje ASCII (American Standard Code for Information Interchange) koji
definira 128 znakova za potrebe teksta na računalu.

Svaki znak je dakle kodiran sa 7 bitova što automatski znači i
memorijsko zauzeće. Od ovih znakova njih 94 su znakovi s vizualnom
reprezentacijom (eng. *printable characters*). To su 26 slova engleske
abecede u malim i velikim varijantama (i.e. 72 slova), 10 arapskih
znamenki, 32 interpunkcijska znaka i 32 kontrolna znaka (od kojih je
većina zastarjela). Svi znakovi osim kontrolnih su prikazani u Tablici
[\[tab:ASCII\]](#tab:ASCII){reference-type="ref" reference="tab:ASCII"}.

``` center
```

Tablica ne sadrži znakove koji nemaju vizualnu reprezentaciju na način
na koji to imaju slova, brojevi i interpunkcija. Među ovim znakovima se
svakako najčešće koristi i najpoznatiji nam je razmak. U suvremenijim
standardima postoje više vrsta razmaka i ova vrsta znakova se naziva
\"prazan prostor\" (eng. *whitespace*) u koji pripadaju i znakovi za
novi redak kao i tabulator (razmak varijabilne dužine).

Kako bi dobili dojam što su razni kontrolni znakovi, zanimljivo je
spomenuti znakove s kojima i danas označavamo prelazak u novi redak. To
su znakovi *carriage return* i *line feed*. Kada se na ovakve znakove
želimo referirati u tekstu običnim znakovima to tipično činimo kroz\
r ili CR (*carriage return*) i\
n ili LF (*line feed*). Na Windows sustavima se kraj retka označava s
oba ova znaka (\
r\
n), a na UNIX sustavima samo sa\
n. Većina suvislog softvera za rad s običnim tekstom će znati tretirati
oba stila pa se oko ovoga ne trebamo previše zabrinjavati. Ono što je
zgodno znati je da kada stisnemo tipku *enter* odnosno *return* kako bi
prešli u novi redak da je ono što računalo zapravo učini je da umetne
ove znakove u tekst. Kao što smo već ranije rekli, tekstualni zapis
zapravo nema koncepte \"redaka\" već je jedan neprekinuti niz znakova.
On jednostavno koristi kontrolne znakove koji označavaju \"ovdje je
prijelaz u novi redak\". Ali sve to nam još uvijek ne govori *što* su ti
znakovi. Odakle potiču? Potiču s pisaće mašine i sličnih tehnologija.

Na posve mehaničkim modelima, valjak na pisaćoj mašini se pomiče kako
tipkamo te ga je na kraju retka potrebno vratiti na početnu poziciju.
Ovo je *carriage return*. Zatim ga je potrebno zarotirati kako bi prešli
u novi redak. Ovo je *line feed*. Ovi koncepti su zakodirani kao znakovi
te ih i danas koristimo na suvremenim računalima za prelazak u novi
redak.

U svakom slučaju, ASCII standard je definirao šifrarnik koji je
propisivao 7-bitne šifre za znakove i tako je podržavao njih 128. Među
ovim šiframa su se nalazila samo slova engleske abecede, a i bez previše
razmišljanja znamo da na svijetu postoji puno puno više od 128
različitih znakova.

Ovakav šifrarnik nazivamo **kodna stranica** (eng. *code page*). To je
dakle šifrarnik putem kojeg računalo prevodi niz nula i jedinica u neki
znak.

### Prošireni ASCII

ASCII standard zapravo nije razvijen za računala već za telegrafiju.
Nedostaju mu koncepti potrebni čak i za engleski jezik kao što su to
posebni znakovi za oblikovanje teksta, više vrsta razmaka i matematički
simboli poput ≠, ≥ i ≈. U 1970-ima su računala standardizirala dužinu
bajta kao 8 bitova. To je otvorilo i put 8-bitnim kodnim stranicama koje
omogućuju duplo više znakova ($2^8 = 256$) no što je to omogućavao
ASCII. Ipak, 256 znakova je još uvijek drastično malen broj kada bismo
pokušali napraviti kodnu stranicu koja bi zadovoljavala potrebe više
naroda s različitim abecedama odjednom. Ovo posebno vrijedi kod naroda
koji ne koriste latinično pismo. ASCII tablicu kao i američku proširenu
ASCII tablicu možemo lako naći *online* u različitim oblicima (tablica,
tekst, slika), jedan od kojih je dostupan
[ovdje](https://www.ascii-code.com).

Prva strategija kojom se ovo krenulo rješavati je tako što se razvio
veliki broj kodnih stranica koje su najčešće koristile 128 znakova
propisanih ASCII-em te dodatnih 128 znakova koje su ovisile o jeziku i
računalu. Ove kodne stranice, međutim nisu standard poput ASCII-a, već
su ih razvijale tvrtke koje su razvijale komercijalne računalne sustave.
Među njima su nam vrlo poznata imena poput IBM, Microsoft i Apple.

### Kaos u kodiranju

Na ovaj način je međutim nastao kaos u kodiranju teksta. Najveći problem
je bio to što tekstualna datoteka odnosno običan tekst u računalnoj
memoriji ne sadrži eksplicitan zapis koju kodnu stranicu neki tekst
koristi već računalo to pretpostavlja iz opće prihvaćenih standarda i
lokalnih postavki sustava. Prema
[Wikipediji](https://en.wikipedia.org/wiki/Extended_ASCII), tokom godina
je razvijeno više od 220 DOS i Windows kodnih stranica koje je razvijao
Microsoft i više nego 186 EBCDIC kodnih stranica koje su IBM-ova inačica
kodnih stranica. A to su samo neke od definiranih kodnih stranica. Kada
se slučajno koristila kriva kodna stranica za dekodiranje, neka slova bi
se zamijenila za druge znakove ili za kriva slova!

Radi ovoga još dan danas u određenim uvjetima možemo vidjeti krive
znakove za hrvatska slova, kao što je to slučaj na npr. računima i malim
ekranima na različitim automatima. Dugo godina se radi toga povlačila
navika da se tekst na hrvatskom (na primjer prilikom pisanja
elektroničke pošte) zapisivao bez palatala, odnosno \"č\" i \"ć\" su se
pisali kao \"c\", a \"š\" kao \"s\". U suprotnom bi se znakovi prečesto
\"raspali\" u prijenosu i postali nešto nečitljivo ili jednostavno posve
druga slova.

Drugim riječima, bio je čest slučaj da se kodnu stranicu trebalo
nagađati i da su se znakovi krivo dekodirali. U ovakvom sustavu je bilo
teško raditi pa se pojavila ideja univerzalne kodne stranice. Također,
računala su postajala sve brža, a memorija sve veća pa je i štednja
memorijskog prostora za potrebe teksta postajala sve manji problem. U
tom smislu nastaje UNICODE, pokušaj da se popišu svi znakovi na svijetu.

### UNICODE

Kažu da je za pročitati novine na suvremenom kineskom potrebno znati 2-3
tisuće znakova. Ovo je samo po sebi već znatno više no što to dopuštaju
8-bitne kodne stranice. Kada pridodamo tome da je moguće lako zamijeniti
putem koje je kodne stranice tekst kodiran i tako pogrešno
interpretirati znakove nameće se sljedeće rješenje: popisati sve znakove
na svijetu.

[UNICODE](https://home.unicode.org) (*Universal Coded Character Set*) je
međunarodni standard koji se trudi popisati sve znakove na svijetu. To
je katalog svih znakova na svijetu koji svakom znaku dodjeljuje
jedinstvenu oznaku bez obzira na različiti hardver i softver koji
koristi. UNICODE 12.1 sadrži podatke o 137 994 različitih znakova. Svaki
znak ima svoj kontrolni broj putem kojeg se možemo nedvojbeno referirati
na neki znak.

Koliko bajtova nam je dakle potrebno da bi zakodirali sve UNICODE
znakove za potrebe računala. Kao što već znamo, jedan bajt je osam
bitova. U osam bitova stane $2^8$ različitih kombinacija, odnosno na
ovaj način možemo prikazati 256 brojeva pa tako i 256 znakova. U 16
bitova stane 65 536 znaka. Ipak, UNICODE ima više od toliko znakova pa
dva bajta nisu dovoljna. Kada bi koristili 32 bita omogućili bi 4 294
967 296 znakova! E to nam je daleko više nego dovoljno za sve znakove na
svijetu i ostavlja dovoljno prostora za dodavanje novih znakova. Kada bi
svakom UNICODE znaku dodijelili njegovu brojčanu šifru, dobili bi
kodiranje koje za svaki znak koristi 4 bajta. Ova kodna stranica se
naziva UTF-32.

Ovo bi dakle riješilo problem. Ipak, ovakav pristup ima dva
fundamentalna nedostatka:

1.  Svaki tekst zauzima četiri puta više mjesta u memoriji (što utječe i
    na prijenos podataka npr. putem interneta)

2.  Najčešća slova u mnogim tekstovima, poput \"e\" i ostalih slova
    zajedničkih svim latiničkim pismima, više nisu kompatibilna sa
    starijim, efikasnijim načinom zapisivanja

U praksi se primijetilo da se znakovi iznad šifre 65 536 koriste vrlo
rijetko pa je napravljena i druga kodna stranica za UNICODE koja može
zakodirati samo prvih 65 536 znakova i koristi dva bajta informacija.
Ova kodna stranica se zove UTF-16. Ona dakle za duplo smanjuje potreban
prostor u memoriji po znaku, ali oba problema su još uvijek prisutno.
Iako je prvi problem umanjen za duplo, to je još uvijek više duplo više
memorije no što je potrebno za čuvanje i prijenos teksta zakodiranog u
8-bitnoj kodnoj stranici.

Također, postoji i problem da različite arhitekture hardvera računala
pohranjuju bajtove u različitom redoslijedu pa UTF-32 i UTF-16 moraju
razrješavati ovaj problem koristeći se posebnim početnim znakom. Detalji
nam ovdje nisu potrebni, ali ovaj problem demonstrira kako u nekim
slučajevima postoje i manje očiti problemi kod kodnih stranica.

### UTF-8

UTF-8 je kodna stranica za UNICODE koja rješava probleme UTF-16 i UTF-32
i danas je *de facto* standard za kodiranje teksta, posebno kada se radi
o web stranicama. Naime kod web stranica je kodna stranica formalno
deklarirana i javno su dostupne pa je ovo bilo lako istražiti, kao što
se vidi npr. na
[ovom](https://en.wikipedia.org/wiki/UTF-8#/media/File:Utf8webgrowth.svg)
grafikonu.

UTF-8 rješava primarni problem kodiranja UNICODE-a tako što svakom znaku
dodijeljuje varijabilan broj bajtova. Na taj način je svim znakovima
definiranim u ASCII-u dodijeljen jedan bajt koji odgovara ASCII kodnoj
stranici. Drugim riječima, ako imamo tekst koji ne koristi niti jedan
znak koji nije definiran ASCII-em, tada je UTF-8 kodirani tekst
identičan ASCII kodiranom tekstu.

Za znakove koji nisu u ASCII standardu, UTF-8 koristi više bajtova.
Znakovi iz fonetskih pisama i dodatna interpunkcija tipično zauzimaju
dva bajta. To je i slučaj s hrvatskim slovima č,ć,đ,š i ž. Ostali
znakovi, poput kineskog pisma zauzimaju tri bajta.

Radi ove mogućnosti u ovaj tekst možemo zapisati i ovo:
不鸣则已，一鸣惊人 (U slobodnom prijevodu, \"Ptica ne pjeva zato jer zna
odgovore već zato jer zna pjesmu.\").

Drugim riječima, **najvažnija kodna stranica danas, koja rješava
probleme razmjene teksta** je **Najčešća slova u mnogim tekstovima,
poput \"e\" i ostalih slova zajedničkih svim latiničkim pismima, više
nisu kompatibilna sa starijim, efikasnijim načinom zapisivanja** i
preporuka je koristiti ovu kodnu stranicu prilikom pisanja bilo kakvog
teksta, bez obzira da li se radi o običnoj tekstualnoj datoteci, e-mail
poruci, zapisu HTML-a ili Pythona i drugog programskog kôda.

Sada kad bolje razumijemo koncept digitalnog elektroničkog teksta i
obične tekstualne datoteke, pogledajmo kako se s njime radi u Pythonu.
