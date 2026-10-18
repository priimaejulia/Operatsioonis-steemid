# Praktikum nr 5

Operatsioonisüsteemide kursuse viiendas praktikumis tutvusin Linuxi protsesside ja signaalide toimimisega, õppisin suunama protsesside sisendeid ja väljundeid, ühendama käske torude abil. Lisaks sain ise protsesse peatada, katkestada ja tappa. 

# ülesanne 5-1:
<img width="382" height="373" alt="ülesanne 5-1" src="https://github.com/user-attachments/assets/688eca90-849b-404b-a7fd-9f49cac1b1e0" />

# ülesanne 5-2:
<img width="406" height="515" alt="ülesanne 5-2" src="https://github.com/user-attachments/assets/ecb1d158-326f-4d0d-9b8b-4a1b28e8fb14" />




# ülesanne 5-3: 
käsujada on ps -axu | grep daemon | grep -v grep | tr -s " " | cut -d" " -f11- | grep daemon

<img width="344" height="326" alt="ülesanne 5-3" src="https://github.com/user-attachments/assets/a2bdf6d7-2c0b-410d-811c-1faa22af0ff7" />





# ülesanne 5-4: 
käsujada on ip a | grep "inet " | grep -v 127.0.0.1 | tr -s " " | cut -d" " -f3 | cut -d"/" -f1

<img width="343" height="320" alt="ülesanne 5-4" src="https://github.com/user-attachments/assets/b2fc03ec-b870-414b-90f5-9c8d453fdd97" />




# ülesanne 5-5: 
A) failis teatedOut.txt valisin välja kaks sõnumit:
1) WM_COMMAND ( logi rida 16:39:16.699, 273, "WM_COMMAND", 996, 394212):
- tekib kolmel juhul: kui kasutaja valib menüüst käsu, juhtelement saadab vanemaknale teavituse või kiirklahvivajutus tõlgitakse. 
- tekkis sellest, et klõpsasin aknas nupule WM_NULL,10,10.
wParam: nupu ID ja teavituskood
lParam: nupu aknakäepide ( ingl a handle to the control window)
  
 https://learn.microsoft.com/en-us/windows/win32/menurc/wm-command
  

2) WM_MOUSEACTIVATE (logi rida 16:39:16.610, 33, "WM_MOUSEACTIVATE", 394222, 33619969)
- tekib kui kursor on mitteaktiivses aknas ja kasutaja vajutab hiirenuppu. 
- tekkis, kuna vajutasin hiirenuppu mitteaktiivses aknas.
wParam: aktiveeritava peaakna käepide ( ingl a handle to the top - level parent window) 
lParam: kursori asukoht ja vajutatud hiirenupp


https://learn.microsoft.com/en-us/windows/win32/inputdev/wm-mouseactivate

B) Proovi tekitada vähemalt 1 sõnum, mida pole tõlketabelis (failis teatedOut.txt on nimeks "???") ja ID on väiksem kui 45000. Millise(d) suutsid tekitada? Suutsin tekitada WM_DPICHANGED (736).


https://learn.microsoft.com/en-us/windows/win32/gdi/wm-displaychange
