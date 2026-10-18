# Praktikum nr 5
ülesanne 5-3: käsujada on ps -axu | grep daemon | grep -v grep | tr -s " " | cut -d" " -f11- | grep daemon
ülesanne 5-4: käsujada on ip a | grep "inet " | grep -v 127.0.0.1 | tr -s " " | cut -d" " -f3 | cut -d"/" -f1
