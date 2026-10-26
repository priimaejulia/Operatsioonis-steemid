# Praktikum nr 6


# ülesanne 6-1:

a) kaust --x (100), fail r--(400)


b) kaust -wx(300), fail ---(000)


# ülesanne 6-2:

Skript on tekstifail, kuhu on käsud järjest kirja pandud. Skripti käivitamisel avab bash skriptifaili ja loeb käsud ükshaaval läbi.Selleks peab bashil olema õigus skripti sisu lugeda. 

Lisaks x  - õigusele on vaja lugemisõigust (r).


# ülesanne 6-3:

Iga kasutaja saab omale privaatrgrupi, et tema failid kuuluksid gruppi, kus on ainult tema. 
Tavakasutaja umask 0002 annab grupile kirjutusõiguse, aga kuna grupis pole kedagi teist, siis ei saa teised kasutajad faile muuta. 

# ülesanne 6-4: 


<img width="476" height="559" alt="ülesanne 6-4" src="https://github.com/user-attachments/assets/ec8e4f6a-1d80-4ae0-9182-252d5a20e575" />






# ülesanne 6-5:




<img width="354" height="121" alt="ülesanne 6-5" src="https://github.com/user-attachments/assets/01413c95-ecae-4c76-9eb0-30f12c4a00e4" />



# ülesannne 6-6: 

Setuid -i kasutamine võib süsteemi turvalisust tõsta või vähendada. 
Ühelt poolt setuid - õigus võimaldab tavakasutajal käivitada programmi faili omaniku õigustes, mitte enda õigustes. Siis saab kasutaja teha ühe kindla piiratud toimingu, ilma et kasutaja peaks saama ligipääsu kogu failile või süsteemile. Näiteks saab vaadata ainult oma lapse hindeid või muuta parooli, ilma et talle antaks otsest ligipääsu kaitstud failidele. 
Teiselt poolt töötab see programm sageli root'i õigustes. Kui programmis on mingi viga, siis võib ründaja selle ära kasutada ja saada root'i õigused, millega ründaja saada täieliku kontrolli kogu süsteemi üle.



# ülesanne 6-7:
Sticky bit'iga saavad kataloogist /tmp/yhiskaust kustutada peetri loodud faile peeter ise , kuna on faili omanik, õpetaja, kuna ta on kataloogi /tmp/yhiskaust omanik, ja root, kuna root on süsteemiadministraator ja tema suhtes failiõigused ei kehti.  


# ülesanne 6-8: 

ls -la väljundis tekkis õiguste lõppu + märk, mis näitab, et failil on ACL-õigused. Grupi õiguste kohal näidatakse nüüd ACL- i maski (rw-). 
Täpsemad õigused on näha käsuga getfacl: grupile direktor on antud lugemis - ja kirjutamisõigus, samas grupil opetaja ei ole ühtegi õigust.


<img width="329" height="193" alt="ülesanne 6-8" src="https://github.com/user-attachments/assets/4205915e-76d4-4ccd-87f6-1f596703c56b" />


# ülesanne 6-9:

- +i atribuudiga faili ei saa muuta mitte keegi, sealhulgas root ei saa muuta.
  
- kustutada saab:
  -> sudo chattr -i testfail-2
  -> sudo rm testfail-2

