# Oppdrag_1

## Nettverk og tilkobling
Jeg klarte å gi en statisk ip adresse til serveren (Rassberry pi).
<img width="743" height="621" alt="image" src="https://github.com/user-attachments/assets/73de749c-d65d-4f80-ad91-7e7f78b66c0e" />


Jeg hadde 10.200.14.22 som statisk ip adresse og klarte å pinge serveren fra bærbar pcen.

<img width="850" height="232" alt="image" src="https://github.com/user-attachments/assets/1739540b-daf9-46c8-b4fd-1c51ac97906a" />

jeg klarte også å pinge bærbar pcen fra serveren.  


## Server og tjeneste
Jeg brukte apace for å gjøre denne oppgaven.

JEg først startet en apache server på Rasberry Pi ved å gjøre disse komandoene: 
- sudo systemctl start apache2
- sudo systemctl enable apache2

Også sjekket jeg om det fungerte ved å søke localhost/ i min søkemotor
<img width="805" height="434" alt="image" src="https://github.com/user-attachments/assets/4a4edda7-e845-4771-b625-8f77fd1ea72e" />

Jeg søkte på statisk ip adressen til Rasberry Pi'en (10.200.14.22) på et annen maskin for å sjekke om jeg kunne åpne localhost nettsiden der og det fungerte.
<img width="800" height="600" alt="image" src="https://github.com/user-attachments/assets/dc1fc750-e203-442e-a8f6-37eefaf5df4b" />


jeg også brukte samba til å ha fildeling mellom linux og windows.

Jeg lastet ned sambe ved å skrive "sudo apt install samba" i bash.

Jeg lagde en mappe som het b"ruh" i min "hjem" directory ved å skrive "mkdir /home/supremekafle/bruh/". Jeg gjorde dette fordi det er den mappen som jeg skal dele med windows.

For at samba vet at jeg vil dele "bruh" mappen, måtte jeg gå inn i sudo config files ved å skrive "sudo nano /etc/samba/smb.conf" og skrive denne kodelinjen på bunnen:
<img width="563" height="157" alt="image" src="https://github.com/user-attachments/assets/b8e9041f-774b-4048-b05f-3a67b5716bc7" />

Jeg ble ferdig med ubuntu delen, nå var det bare windows delen igjen.

Windows delen var mye enklere enn Ubuntu fordi alt man måtte gjøre var:
-gå inni file explorer
-bytte filepath til \\ + ip adressen min, så det var \\10.200.14.22



## Python og Github
Det første jeg gjorde var at jeg lagde en veldig enkel python script som viser systeminformasjon i visual studio code. 
<img width="560" height="168" alt="image" src="https://github.com/user-attachments/assets/407788b3-61ef-41cc-80c1-393a9db4f954" />

Jeg legget den python filen i github fra laptopen og lastet den ned inni i Documents folder på Rassberyy Pi ved å gjøre "cd Documents" og "git clone" kommandoene.
<img width="855" height="206" alt="image" src="https://github.com/user-attachments/assets/6d614ab7-8767-4f0e-9b85-21b0314fa916" />

Jeg gjorde "ls" kommandoen mens jeg var i documents for å finne ut hva den nye mappen het.
<img width="855" height="50" alt="image" src="https://github.com/user-attachments/assets/a44d98c4-747a-46af-8baf-429642e204ad" />

Jeg fant ut at nye mappen het "Oppdrag_1" på grunn av dette.

Jeg gikk inn i den nye mappen ved å gjøre "cd Oppdrag_1". Jeg måtte gå inn i mappen fordi da kan jeg endelig kjøre python filen som er inni den ved å gjøre python3 kommandoen.

Jeg vet allerede at python filenmin heter "Systeminfo.py", så jeg gjorde "python3 Systeminfo.py" og det fungerte.
<img width="851" height="114" alt="image" src="https://github.com/user-attachments/assets/0b7a8af0-3e6c-4967-b097-6a3530ea10bb" />








