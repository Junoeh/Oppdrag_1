# Oppdrag_1

## Nettverk og tilkobling
Jeg klarte å gi en statisk ip adresse til serveren (Rassberry pi). Jeg hadde 10.200.14.22 som statisk ip adresse og klarte å pinge serveren fra bærbar pcen.

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

