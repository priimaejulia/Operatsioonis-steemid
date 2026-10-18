# Praktikum nr 5
# ülesanne 5-3: käsujada on ps -axu | grep daemon | grep -v grep | tr -s " " | cut -d" " -f11- | grep daemon



# ülesanne 5-4: käsujada on ip a | grep "inet " | grep -v 127.0.0.1 | tr -s " " | cut -d" " -f3 | cut -d"/" -f1



# ülesanne 5-5: failis teatedOut.txt valisin välja kaks sõnumit:
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
