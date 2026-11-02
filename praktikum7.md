# Praktikum nr 7 

# ülesanne 7-1:

Uus andmekandja on alguses täiesti tühi ja operatsioonisüsteem ei oska seda kasutada, kuna sellel puudub nii partitsioonitabel kui ka failisüsteem. Süsteem ei tea, kus partitsioonid algavad ja lõpevad ning kuidas faile salvestada. Lähtestamisel kirjutatakse kettale partitsioonitabel (MBR või GPT), mis näitab ketta osadeks jaotumist. Üle 2 TB ketaste puhul tuleks kasutada GPT-d, sest MBR ei toeta nii suuri kettaid. Seejärel luuakse vormindamisel partitsioonile failisüsteem (nt NTFS või ext4), mis hoiab arvet selle üle, kus failid kettal asuvad ja kui palju vaba ruumi on. Alles siis saab ketta süsteemiga ühendada ja sinna faile salvestada.

# ülesanne 7-2:



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
