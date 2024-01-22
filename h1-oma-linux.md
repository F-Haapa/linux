# h1 - Oma Linux

Aloitin harjoituksen tekemisen maanantaina 22.1.2024 noin klo 19 soluasunnossani koneenani suoraan paketista kiskottu Asus ROG Flow X13 ja käyttöjärjestelmänä Windows 11 versio 21H2.

Käynnistin VirtualBoxin, valitsin valikosta 'Machine' vaihtoehdon 'New', jonka jälkeen avautui uusi ikkuna 'Create Virtual Machine'.

![kuva](/kuva01.png)

Ikkunan kenttiin täytin seuraavat tiedot:

'Name and Operating system'
- Name: Debian
- Folder: C:\Users\fanny\VirtualBox VMs
- ISO Image: C:\Users\fanny\Downloads\debian-live-12.4.0-amd64-xfce.iso
- Type: Linux
- Version: Debian (64-bit)
- ✓ Skip Unattended Installation.

[kuva]

'Hardware'
- Base Memory: 6000 MB
- Processors: 2

[kuva]

'Hard Disk'
- Create a Virtual Hard Disk Now
	'Hard Disk File Location and Size'
	- Folder: C:\Users\fanny\VirtualBox VMs\Debian\Debian.vdi
	- 60,00 GB
	'Hard Disk File Type and Variant'
	- VDI (VirtualBow Disk Image)

[kuva]

Lopuksi painoin 'Finish'-nappia.

[kuva]

Kaksoisklikkasin uutta virtuaalikonetta.

[kuva]

Bootloader avautui, valitsin ensimmäisen vaihtoehdon painamalla enter.

[kuva]

Klikkasin painiketta 'Applications' ja valitsin valikosta 'Web Browser'. Kirjoitin osoitekenttään "tero karvinen" ja painoin enter. Klikkasin ensimmäistä linkkiä ja pääsin Tero Karvisen nettisivuille.

[kuva]

Suljin selaimen painamalla x selaimen oikeasta yläkulmasta.

Kaksoisklikkasin työpöydällä olevaa 'Install Debian' -kuvaketta.
Sain seuraavan ilmoituksen:

[kuva]

En reagoinut ilmoitukseen tarpeeksi nopeasti, ja sain seuraavan virheilmoituksen.

[kuva]

Painoin 'Launch Anyway', ja 'Debian GNU/Linux Installer' -ikkuna avautui. Suurensin ikkunan painamalla neliötä ikkunan oikeasta yläkulmasta.

Asennusohjelma ehdotti kieleksi 'American English', en tehnyt muutoksia ja painoin 'Next'.

Seuraavalla sivulla ('Location') klikkasin kartasta Suomea, jolloin ohjelma täytti kohtiin 'Region': Europe ja 'Zone': Helsinki.

Painoin 'Next'.

Seuraavalla sivulla ('Keyboard') valitsin vasemmanpuoleisesta valikosta 'Finnish' ja oikeanpuoleisesta 'Default'.

Painoin 'Next'.

Seuraavalla sivulla ('Partions') valitsin vaihtoehdon 'Erase disk', jolloin sivun alareunaan tuli lisävalintoja, mutta en koskenut niihin.

Painoin 'Next'.

Seuraavalla sivulla ('Users') täytin kentät seuraavanlaisesti:
'What is your name?'
- Fanny Haapa
'What name do you want to use to log in?'
- fannyh
'What is the name of this computer?'
- keksi
'Choose a password to keep your account safe.'
- Kirjoitin 9-merkkisen salasanan jossa on sekalaisesti kirjaimia, numeroita ja erikoismerkkejä kahteen kertaan. Kirjoitin salasanan uudelleen kahteen kertaan koska salasanat eivät täsmänneet.

Painoin 'Next'.

Seuraavalla sivulla ('Summary') painoin 'Install'.
Asennus alkoi ja kesti noin 4-5 minuuttia.

✓ Restart now

Painoin 'Done'.

Muutaman minuutin ajan ei tuntunut tapahtuvan mitään, mutta sitten kone käynnistyi ja login screen aukesi.

Kirjauduin sisään.

Testasin toimivuutta samalla tavalla kuin aiemminkin:
"Klikkasin painiketta 'Applications' ja valitsin valikosta 'Web Browser'. Kirjoitin osoitekenttään "tero karvinen" ja painoin enter. Klikkasin ensimmäistä linkkiä ja pääsin Tero Karvisen nettisivuille."

Klikkasin painiketta 'Applications' ja valitsin valikosta 'Terminal Emulator', komentorivi avautui. Kirjoitin komennon

"sudo apt-get update"

jolloin ohjelma kysyi salasanaa, jonka kirjoitin (salasana ei näkynyt kirjoitettaessa) ja painoin enter.

Muutaman minuutin päästä komento oli käsitelty.

$ sudo apt-get -y install ufw
Palomuuri päälle
$ sudo ufw enable

Klikkasin painiketta 'Applications' ja valitsin valikosta 'Log out'.
Uusi ikkuna aukesi, painoin 'Restart'.

Kello oli 20:50. Harmillisen suuri osa käytetystä ajasta meni tapellessa uuden näppäimistön ja uuden läppärin asetusten kanssa, mutta en sisällyttänyt sitä tähän raporttiin koska se ei liittynyt tehtävään.
