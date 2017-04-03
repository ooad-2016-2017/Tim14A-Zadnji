## Tim14A-Zadnji

# **VAŠ GRAS**

Članovi tima:
  1. Selma Gutošić
  2. Ahmed Serdarević

## Opis teme

**VAŠ GRAS** je aplikacija koja je zamišljena s ciljem omogućavanja korisnicima javnog gradskog prevoza jednostavniji način kupovine prevoznih karata, jednostavnije korištenje usluga prevoza, te mogućnost saznanja pozicije kretanja vozila GRAS-a. Danas čovječanstvo živi brz tempo života. Neophodno je imati mnogobrojne informacije trenutačno, jer naše odluke zavise od kvalitetnih informacija koje posjedujemo, a s obzirom na taj isti tempo kojim živimo, možemo reći da je jedna istina apsolutna danas. Suočeni smo sa nedostatkom vremena. Što bi rekli naši stari: 
>Nema sinko više bereketa u vremenu.

Upravo pomoću ove aplikacije korisnici će moći elektronski kupiti karte za gradski saobraćaj, s mogućnošću biranja optimalnog broja vožnji koji im odgovara. Omogućena će biti kupovina različitog tipa karti (dnevne, sedmične, mjesečne godišnje, proizvoljan broj vožnji(10,20 i ...)). Korisnici prilikom ulaska u prevozno sredstvo će pomoću RFID tehnologije se "prijaviti/čekirati", te će ovisno o stanju njegovog računa odgovarajući hardver(koji se nalazi u sklopu prevoznog sredstva) omogućiti prolazak putniku, ili će u slučaju da je njegova karta istekla signalizirati neophodnost da kupi kartu kod vozača. Na ovaj način interakcija vozača i putnika bi bila svedena na minimum, a putnici se ne bi zadržavali i stvarali gužve bespotrebno pri ulasku u prevoyno sredstvo. Također sva vozila će biti povezana sa sistemom, te će prilikom ulaska u vozilo, putnici imati uvid pomoću aplikacije o stanju vozila(godište, posljednja dezinfekcija, dezinsekcija i deratizacija, trenutni vozač itd) te će moći dati svoju ocjenu kako vozaču koji upravlja vozilom tako i samom vozilu. Ukoliko neko smatra da ne postoji potreba za vođenjem bilo kakve evidencije o vožnji vozača, savjetujem im da iskoriste GRASV-u **_15-ku_**.
Također s obzirom da će sva vozila biti povezana GPS-om, korisnici će biti u mogućnosti pratiti pozicije prevoznih sredstava koja rade na željenoj liniji, te na taj način isplanirati tačan dolazak na stanicu. 

## Procesi

* Registracija i prijava korisnika: Osoba podnosi zahtjev za kreiranje korisničkog računa. Neophodni podaci za kreiranje korisničkog računa su:
  * Ime
  * Prezime
  * Matični broj
  * Status osobe(učenik, student, zaposlen/nezaposlen, uposlenik firme)
  * Šifra(osoba prilikom registracije unosi svoju šifru i čeka potvrdu registracije)
  * Ukoliko je uposlenik GRAS-a, osoba dobija dodatni sigurnosni kod. 
Unos podataka vrši administrator koji ujedno i izdaje RFID senzore svima koji se registruju. Registracija košta 10 KM.   

* Kupovina karata: Osoba nakon registrovanja korisničkog računa za aplikacij može odabrati željeni tip vozne karte koju želi kupiti, kao i vremenski termin kupovine. U ponudi će imati više tipova karata (dnevna, sedmična, mjesečna, godišnja, proozvoljan broj vožnji). Osoba nakon odabira tipa karte koju želi kupiti, odlazi na prodajno mjesto JKP Gras-a u određenom željenom terminu, te izvrši plaćanje karte osobi koja radi na naplati karata.

* Prijava vozača: Vozač prilikom ulaska u vozilo, prijavljuje se na aplikaciju. Prilikom prijave aplikacija traži unos sigurnosnog koda koji svaki od uposlenika dobiva pri registraciji. Također vozač vrši prijavu vozila isto tako sa sigurnosnim kodom. Razumijemo da će svako prevozno vozilo biti opremljeno jednim mobilnim uređajem, sa kojim će biti povezano na aplikaciju. 

* Prilikom ulaska u prevozno sredstvo dovoljno je da osoba potvrdi svoj ulazak RFID uređajem. Ukoliko putnik nije iskoristio svoju kartu, senzor potvrđuje mogućnost njegovog prolaska. Međutim ukoliko pri ulasku u vozilo senzor očita da stanje njegovog računa nije zadovoljavajuće(tj. osoba nema kartu, ili je ista istekla) putnik onda mora kupiti kartu kod vozača.

* Uvid u položaj trenutni položaj vozila: soba nakon prijave na aplikaicju može odabrati željenu liniju vožnje. S obzirom da su sva vozila povezana sa sistemom, prate se informacije o položaju vozila u toku vožnje pomoću GPS-a. Na taj način osoba može isplanirati tačan dolazak na stanicu, jer ima uvid u lokaciju svih vozila koja voze na željenoj relaciji. (Drugi način je da pri svakom dolasku na stajalište vozač da signal da se nalazi na stajalištu. Npr ukoliko neka linija ima 10 stajališta u oba smijera, vozač može signalizirati na aplikaciji prvo u kojem se smijeru kreće, a zatim prilikom dolaska na svaku od stanica signalizirati svoj dolazak. Samim proračunom nije teško odrediti posljenju lokaciju vozila, međutim moramo se osloniti da vozač nikada neće pogriješiti tj. zaboraviti signalizirati svoj dolazak. Iako je ovaj način lakše implementirati od GPS-a, on sa sobom nosi vjerovatnoću greške. Ona se može otkoloniti ako proračunamo prosječno trajanje vožnje u jednom smijeru, te odredimo mogućnost da aplikacija signalizira vozaču svaki put kada bi trebao da se nalazi na krajnjoj stanici. Tada on treba restovati poziciju, te ponovo otpočeti čekiranje na svakoj od sljedećih stanica u narednom krugu vožnje.

* Ocjenjivanje usluge: Svakako rješenje za nesavjesne vozače se ogleda u ocjenjivanju usluge. Nakon što osoba uđe u prevozno sredstvo, ona ima uvid u stanje vozila u kojem se nalazi, te vozaču koji upravlja vozilom. Ukoliko je vozač kasnio ili je vozio nesavjesno, putnici će moći ocijeniti samu uslugu. Pri ocjenjivanju bit će ponuđene opcije:
  * Ocijena vozača (1-5)
  * Ocijena vozila (1-5
 Također će putnici moći ostaviti komentar vezano za vozilo/ vozača i uslugu.

* Postavljanje obaviještenja od strane vozača: Ukoliko vozač ima potrebu da obavijesti sve putnike na svojoj liniji o situaciji u saobraćaju obaviještava kontrolera saobraćaja o situaciji. Kontrolor saobraćaja zatim unosi to obaviještenje na aplikaciju, te sve zainteresirani putnici mogu pročitati obavijest.

## Funkcionalnosti

* Mogućnost kupovine karata
* Mogućnost korištenja prevoza uz minimalnu interakciju sa vozačem
* Mogućnost uvida u pozicije svih vozila 
* Mogućnost uvida u stanje vozila koje koristimo
* Mogućnost ocjenjivanja i kritikovanja usluge gradskog saobraćaja, te samim tim uticanja na kvalitetu istog

## Akteri

**1. Korisnik javnog gradskog prevoza** - Osoba koja koristi gradski prevoz. Mora posjedovati account i broj računa sa kojim će kupovati karte, ukoliko to želi. Također prilikom registracije dobiva RFID senzor koji će koristiti kao identifikator. Ne može se prijaviti u aplikaciju kao uposlenik saobraćaja.

**2. Vozač** - Osoba koja je uposlenik GRAS-a. Neophodno je da se registruje pri ulasku u vozilo, kao i da prijavi samo vozilo u aplikaciju. Osim što upravlja vozilom, on može postavljati obavijesti koje se tiču korisnika prevoza na aplikaciji.

**3. Kontrolor saobraćaja** - Osoba koja upravlja preduzećem. Posjeduje pristup informacijama svih uposlenika, te na osnovu njihovih rejtinga stimuliše ih za njihov kvalitetan rad ili kažnjava za nekvalitetan. Određuje red vožnji, postavlja obavijesti koje se tiču radnika i putnika, postavlja raspored vožnji na aplikaciji, modificaira ih.

**4. Administrator** - Osoba koja je zadužena za održavanje aplikacije. Unosi podatke svih uposlenika, omogućava registrovanje putnika, izdaje svim registriranim korisnicima njihove šifre koje koriste za identifikaciju i osiguravanje identiteta. Dodaje nove uposlenike i uklanja bivše. 

**5. Prodavač/čica** - Osoba koja je zadužena za prodaju karata(potvrdu kupovine karata)

**6. Upravnik** - Osoba koja nadgleda rad uposlenika, te na osnovu ocjene korisnika nagrađuje ili kažnjava vozače
