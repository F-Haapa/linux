# h1 - Oma Linux

Aloitin harjoituksen tekemisen maanantaina 22.1.2024 noin klo 19 soluasunnossani koneenani suoraan paketista kiskottu Asus ROG Flow X13 ja käyttöjärjestelmänä Windows 11 versio 21H2.

Käynnistin VirtualBoxin, valitsin valikosta **Machine** vaihtoehdon **New**, jonka jälkeen avautui uusi ikkuna **Create Virtual Machine**.

![kuva1](/kuva01.png)

Ikkunan kenttiin täytin seuraavat tiedot:

*Name and Operating system*
- Name: Debian
- Folder: C:\Users\fanny\VirtualBox VMs
- ISO Image: C:\Users\fanny\Downloads\debian-live-12.4.0-amd64-xfce.iso
- Type: Linux
- Version: Debian (64-bit)
- ✓ Skip Unattended Installation.

![kuva2](/kuva02.png)

*Hardware*
- Base Memory: 6000 MB
- Processors: 2

![kuva3](/kuva03.png)

*Hard Disk*
- Create a Virtual Hard Disk Now
	'Hard Disk File Location and Size'
	- Folder: C:\Users\fanny\VirtualBox VMs\Debian\Debian.vdi
	- 60,00 GB
	'Hard Disk File Type and Variant'
	- VDI (VirtualBow Disk Image)

![kuva4](/kuva04.png)

Lopuksi painoin **Finish**-nappia.

Kaksoisklikkasin uutta virtuaalikonetta.

![kuva5](/kuva05.png)

Bootloader avautui, valitsin ensimmäisen vaihtoehdon painamalla **enter**.

![kuva6](/kuva06.png)

Työpöytä tuli näkyviin.

![kuva7](/kuva07.png)

Klikkasin painiketta **Applications** ja valitsin valikosta **Web Browser**. Kirjoitin osoitekenttään *"tero karvinen"* ja painoin **enter**. Klikkasin ensimmäistä linkkiä ja pääsin Tero Karvisen nettisivuille.

![kuva8](/kuva08.png)
![kuva10](/kuva10.png)

Suljin selaimen painamalla **x** selaimen oikeasta yläkulmasta.

Kaksoisklikkasin työpöydällä olevaa ***Install Debian*** -kuvaketta.
Sain seuraavan ilmoituksen:

![kuva12](/kuva12.png)

En reagoinut ilmoitukseen tarpeeksi nopeasti, ja sain virheilmoituksen. Suljin virheilmoituksen painamalla **Close**.

![kuva13](/kuva13.png)

Painoin **Launch Anyway**, ja *Debian GNU/Linux Installer* -ikkuna avautui. Suurensin ikkunan painamalla neliötä ikkunan oikeasta yläkulmasta.

Asennusohjelma ehdotti kieleksi 'American English', en tehnyt muutoksia ja painoin 'Next'.

![kuva14](/kuva14.png)

Seuraavalla sivulla (*Location*) klikkasin kartasta Suomea, jolloin ohjelma täytti kohtiin *Region*: Europe ja *Zone*: Helsinki.

Painoin **Next**.

![kuva15](/kuva15.png)

Seuraavalla sivulla (*Keyboard*) valitsin vasemmanpuoleisesta valikosta **Finnish** ja oikeanpuoleisesta **Default**.

Painoin **Next**.

![kuva16](/kuva16.png)

Seuraavalla sivulla (*Partitions*) valitsin vaihtoehdon **Erase disk**, jolloin sivun alareunaan tuli lisävalintoja, mutta en koskenut niihin.

Painoin **Next**.

![kuva17](/kuva17.png)

Seuraavalla sivulla (*Users*) täytin kentät seuraavanlaisesti:

*What is your name?*

- Fanny Haapa

*What name do you want to use to log in?*

- fannyh

*What is the name of this computer?*

- keksi

*Choose a password to keep your account safe.*

- Kirjoitin 9-merkkisen salasanan jossa on sekalaisesti kirjaimia, numeroita ja erikoismerkkejä kahteen kertaan.
- Kirjoitin salasanan uudelleen kahteen kertaan koska salasanat eivät täsmänneet.

Painoin **Next**.

![kuva19](/kuva19.png)

Seuraavalla sivulla (*Summary*) painoin **Install**.

![kuva20](/kuva20.png)

Asennus alkoi ja kesti noin 4-5 minuuttia.

![kuva21](/kuva21.png)

***✓ Restart now***

Painoin **Done**.

![kuva22](/kuva22.png)

Muutaman minuutin ajan ei tuntunut tapahtuvan mitään, mutta sitten kone käynnistyi ja login screen aukesi.

Kirjauduin sisään.

![kuva24](/kuva24.png)

Testasin toimivuutta samalla tavalla kuin aiemminkin:
*Klikkasin painiketta 'Applications' ja valitsin valikosta 'Web Browser'. Kirjoitin osoitekenttään "tero karvinen" ja painoin enter. Klikkasin ensimmäistä linkkiä ja pääsin Tero Karvisen nettisivuille.*

Klikkasin painiketta **Applications** ja valitsin valikosta **Terminal Emulator**, komentokehote avautui. Kirjoitin komennon

> $ sudo apt-get update

jolloin ohjelma kysyi salasanaa, jonka kirjoitin (salasana ei näkynyt kirjoitettaessa) ja painoin **enter**.

![kuva27](/kuva27.png)

Syötin komennon softan päivittämiseksi ja painoin **enter**.

> $ sudo apt-get -y dist-upgrade

Muutaman minuutin päästä komento oli käsitelty.

![kuva29](/kuva29.png)

Asensin palomuurin komennolla:

> $ sudo apt-get -y install ufw

![kuva31](/kuva31.png)

Laitoin palomuurin päälle komennolla:

> $ sudo ufw enable

![kuva32](/kuva32.png)

Seuraavaksi suljin komentokehotteen, klikkasin painiketta **Applications** ja valitsin valikosta **Log out**.
Uusi ikkuna aukesi, painoin **Restart**.

![kuva33](/kuva33.png)

Kone käynnistyi uudelleen.

Kello oli 20:50. Harmillisen suuri osa käytetystä ajasta meni tapellessa uuden näppäimistön ja uuden läppärin asetusten kanssa, mutta ette saa tietää seikkailuistani niiden suhteen koska se ei liittynyt tehtävään.


# Tiivistettyjä pointteja artikkeleista

- muistiinpanot auttavat selkeyttämään asioita, toimivat ohjeiden pohjana, sekä säästävät aikaa ja turhaa asioiden toistamista
- raportin perusteella pitää pystyä toistamaan raportoitu asia, sen on oltava täsmällinen ja helppolukuinen, siinä ei saa olla sepitettyjä asioita eikä plagiointia
- lähteisiin tulee viitata oikein

- vapaa ohjelmisto tarkoittaa että käyttäjät voivat käyttää, kopioida, jakaa, tutkia, muuttaa ja parantaa ohjelmistoa
