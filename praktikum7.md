# Praktikum nr 7 




# ülesanne 7-1:

Uus andmekandja on alguses täiesti tühi ja operatsioonisüsteem ei oska seda kasutada, kuna sellel puudub nii partitsioonitabel kui ka failisüsteem. Süsteem ei tea, kus partitsioonid algavad ja lõpevad ning kuidas faile salvestada. Lähtestamisel kirjutatakse kettale partitsioonitabel (MBR või GPT), mis näitab ketta osadeks jaotumist. Üle 2 TB ketaste puhul tuleks kasutada GPT-d, sest MBR ei toeta nii suuri kettaid. Seejärel luuakse vormindamisel partitsioonile failisüsteem (nt NTFS või ext4), mis hoiab arvet selle üle, kus failid kettal asuvad ja kui palju vaba ruumi on. Alles siis saab ketta süsteemiga ühendada ja sinna faile salvestada.

# ülesanne 7-2:
- rohkem partitsioone ja lihtsam ülesehitus: MBR partitsioonitabelis on ruumi ainult neljale primaarsele partitsioonile, rohkemate jaoks tuleb luua laiendatud partitsioon ja selle sisse loogilised partitsioonid, mis teeb struktuuri keerulisemaks. GTP - s on vaikimisi ruumi 128 partitsioonile ja primaarseid ja loogilisi partitsioone eraldi ei ole. 
- partitsioonitabeli varukoopia: MBR -is on primaarsete partitsioonide tabel ainult ketta esimeses sektoris. Kui see sektor saab kahjustada, ei leia süsteem partitsioone enam üles. GTP hoiab päisest ja partitsioonitabelist varukoopiat ketta lõpus, nii et põhikoopia rikke korral saab tabeli varukoopiast taastada.
- kontrollsummad: GTP päises on CRC32 kontrollsumma nii päise kui ka partitsioonitabeli kohta. Selle abil saab süsteem tuvastada, kas table on rikutud, ning vajadusel kasutada varukoopiat. MBR - is sellist kontrolli ei ole ja rikutud andmeid ei pruugita märgata.
- suurem toetatud kettamaht: MBR suudab kasutada ainult kuni 2TiB suurust kettaruumi. GTP kasutab sektorite numbrite jaoks kaks korda pikemaid aadresse, mistõttu sobivad sellele ka väga suured kettad. 


# ülesanne 7-3: 
https://kodu.ut.ee/~juliapriimae/opsys/hdd.png

# ülesanne 7-4:


<img width="477" height="561" alt="Kuvatõmmis 2026-11-02 090930" src="https://github.com/user-attachments/assets/ff5cf391-0686-43f9-86f7-88dff969aa04" />


# ülesanne 7-5:

Vastus: -o ro haakis andmekandja kirjutuskaitstult. Ma sain faile vaadata, aga mitte kirjutada, muuta ega kustutada. -t auto mõjutas failisüsteemi tüübi valikut: ma ei määranud tüüpi käsitsi, vaid süsteem tuvastas partitsioonilt NTFS-i ja haakis selle sobiva draiveriga. 


# ülesanne 7-6:

Vastus: Ubuntu asendas auto-parameetri väärtusega fuseblk.


# ülesanne 7-7: 




<img width="1101" height="767" alt="ülesanne 7-7" src="https://github.com/user-attachments/assets/275b3a0e-f691-44ee-a54f-dde7b3a7972a" />
