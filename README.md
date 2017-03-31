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
  *Ime
  *Prezime
  *Matični broj
  *Status osobe(učenik, student, zaposlen/nezaposlen, uposlenik firme)
  *Šifra(osoba prilikom registracije unosi svoju šifru i čeka potvrdu registracije)
 



Korisnik aplikacije se prijavi na istu kao korisnik gradskog prevoza. Ukoliko ne posjeduje korisnički račun, otvara isti. Aplikacija poznaje više tipova korisničkih računa (putnik, vozač, poslovođa, administrator, vozilo), te prilikom kreiranja računa bira jedan od ponuđenih tipova. Ukoliko je riječ o putniku, on daje svoje podatke koji su od interesa te čeka odobrenje od administratora (sistema). Sa odobrenjem dobija karakterističnu šifru koju će koristiti pri identifikaciji, kao i RFID senzor. Administrator unosi podatke svih uposlenika GRAS-a, tako da će u slučaju da se običan putnik pokušva prijaviti sa nalogom uposlenika, ista prijava biti onemogućenja, jer svaka od djelatnosti će posjedovati karakterističan kod koji će služiti za identifikaciju. Nakon kreiranja računa, putnik može pomoću aplikacije odabrati tip putne karte koju želi kupiti. U ponudi će biti karte različitog vremenskog perioda korištenja(mjesečna, sedmična, denvna) ili sa konačnim brojem vožnji. Nakon što odabere željeni tip, korisnik aplikacije će plaćanje vršiti elektronskim putem, pomoću _PayPal-a_. Prijavom na aplikaciju, korisnik će moći odabrati željenu liniju koju želi koristiti npr. _Dobrinja-Vijećnica_, te će mu aplikacija izbaciti listu vozila koja voze na toj lokaciji, kao i njihovu posljenju poziciju na kojoj su se ta vozila nalazila. Samim tim će osoba moći kvalitetno rasporediti svoje vrijeme. Prilikom ulaska u prevozno sredstvo, osoba će svoju identifikaciju vršiti RFID uređajem, te će sistem u tom prevoznom sredstvu potvrditi mogućnost prolaska putnika ovisno o stanju njegovog računa. Također putnici će imati pregled stanja vozila, vozača, te dati ocjenu ugođaju vožnje. Što se tiče vozača on će prilikom ulaska u vozilo, također se prijaviti na aplikaciju, prijavit će vozilo koje koristi(napominjemo da svako vozilo će imati karakterističan sistem identifikacije), te u toku vožnje će moći postaviti obavijesti na aplikaciji, npr. Ukoliko se dogodila neka nesreća, vozač će moći postaviti obavijest da se saobraćaj odvija otežano, što svi koji budu u aplikaciji odabrali njegovu liniju saobraćaja će moći vidjeti. Poslovođa će pratiti rejtinge vozača kao i vozila, pratiti će kritike putnika koje će oni postavljati, te će savjesne vozače i odgovorne nagraditi, one malo manje odgovorne kazniti.

## Funkcionalnosti

* Mogućnost online kupovine karata
* Mogućnost korištenja prevoza uz minimalnu interakciju sa vozačem
* Mogućnost uvida u pozicije svih vozila 
* Mogućnost uvida u stanje vozila koje koristimo
* Mogućnost ocjenjivanja i kritikovanja usluge gradskog saobraćaja, te samim tim uticanja na kvalitetu istog

## Akteri

**1. Korisnik javnog gradskog prevoza** - Osoba koja koristi gradski prevoz. Mora posjedovati account i broj računa sa kojim će kupovati karte, ukoliko to želi. Također prilikom registracije dobiva RFID senzor koji će koristiti kao identifikator. Ne može se prijaviti u aplikaciju kao uposlenik saobraćaja.

**2. Vozač** - Osoba koja je uposlenik GRAS-a. Neophodno je da se registruje pri ulasku u vozilo, kao i da prijavi samo vozilo u aplikaciju. Osim što upravlja vozilom, on može postavljati obavijesti koje se tiču korisnika prevoza na aplikaciji.

**3. Upravnik** - Osoba koja upravlja preduzećem. Posjeduje pristup informacijama svih uposlenika, te na osnovu njihovih rejtinga stimuliše ih za njihov kvalitetan rad ili kažnjava za nekvalitetan. Određuje red vožnji, postavlja obavijesti koje se tiču radnika i putnika, postavlja raspored vožnji na aplikaciji, modificaira ih.

**4. Administrator** - Osoba koja je zadužena za održavanje aplikacije. Unosi podatke svih uposlenika, omogućava registrovanje putnika, izdaje svim registriranim korisnicima njihove šifre koje koriste za identifikaciju i osiguravanje identiteta. Dodaje nove uposlenike i uklanja bivše. 

