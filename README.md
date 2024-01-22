# LineFollower

## DOCUMENTAȚIE  PROIECT LINE FOLLOWER (TEI F1)
### ILIE OCTAVIAN TUDOR
### ENESCU HORIA
### TURIS GAVRIIL-VLAD

### Descriere task

În cadrul unui proiect de introducere în robotică, am dezvoltat un robot line follower utilizând un Arduino Uno. Acesta a fost o modalitate excelentă de a învăța și aplica conceptele de bază din robotică.

Robotul este construit pe o structură simplă de carton, asigurând astfel o bază ușoară și accesibilă pentru componentele electronice. Am folosit un breadboard mini pentru a conecta componentele, fire de legătură pentru a facilita conexiunile electrice, și un ball caster pentru a oferi stabilitate robotului.

### Componente

- Arduino Uno: Inima proiectului, utilizat ca unitate centrală de control.
- Breadboard Mini: Pentru a facilita conexiunile electrice.
- Fire de Legătură: Esențiale pentru conectarea componentelor.
- Ball Caster: Pentru mobilitate și echilibru.
- Două Motoare cu Driver L293D: Asigură mișcarea robotului.
- Baterie LiPo: Sursa de alimentare.
- Senzori QTR: Vitali pentru detectarea liniei.

### Cod

https://github.com/VladRo26/LineFollower/blob/main/line_follower.ino

### Design și Construcție

Am construit robotul pe o bază de carton, creând o platformă ușoară și adaptabilă. Am integrat componentele electronice pe breadboard-ul mini, iar motoarele au fost montate pe laterale pentru propulsie. Ball caster-ul a adăugat stabilitate necesară pentru mișcările robotului.

### Partea de software

Am dezvoltat o parte de software în care am inclus biblioteca QTRSensors și am definit pinii pentru motoare și senzori. În cadrul sistemului PID (Proportional-Integral-Derivative), care este esențial pentru controlul mișcării robotului, am adăugat o funcție suplimentară pentru gestionarea erorilor. Această funcție a fost proiectată special pentru a face față situațiilor în care robotul întâlnește curbe pe traseu.

Prin ajustarea fină a valorilor PID - kp, ki și kd - am reușit să asigur o urmărire mai fluidă și precisă a liniei. Însă, pentru a face robotul mai adaptabil la schimbările brusce de direcție, cum ar fi curbele, am implementat un algoritm care ajustează dinamic viteza motoarelor în funcție de magnitudinea și frecvența erorilor detectate. Aceasta înseamnă că, atunci când robotul detectează o curbă, își ajustează viteza motoarelor pentru a o negocia mai eficient, evitând astfel să devieze de la traseu.

Auto-calibrarea, pe care am integrat-o în robot, contribuie și ea la această adaptabilitate, permițând robotului să recunoască diferite tipuri de suprafețe și condiții de iluminat. Acest lucru este crucial în situații unde linia urmată trece de pe o suprafață pe alta sau este afectată de schimbări ale luminii.

### Provocările și Învățăturile

Principalul obstacol a fost ajustarea fină a parametrilor PID - kp, ki și kd - pentru a asigura o urmărire fluidă și precisă a liniei. Auto-calibrarea a adăugat un nivel de complexitate, dar, în același timp, a sporit eficiența și robustețea robotului. Prin depășirea acestor provocări, am dobândit cunoștințe valoroase în domeniul robotic și am dezvoltat competențe în rezolvarea problemelor și lucrul în echipă.

### Fotografii si videoclipuri

#### Fotografii:

Cum arăta înainte sa o dăm de toți pereții:

![WhatsApp Image 2024-01-20 at 15 27 08](https://github.com/VladRo26/LineFollower/assets/100710098/908e3c61-a23b-477f-93e2-2a9c0fcfd0b8=200x200)

Cum arăta după:

![WhatsApp Image 2024-01-21 at 20 37 36](https://github.com/VladRo26/LineFollower/assets/100710098/d193d415-afc3-4a58-8c7b-a29afcd85789=200x200)


![WhatsApp Image 2024-01-21 at 20 37 37](https://github.com/VladRo26/LineFollower/assets/100710098/0572ccb5-5181-4732-ba9f-048b346fc735=200x200)

#### Videoclip (traseul crocodil):

https://www.youtube.com/shorts/5sdWQ27HN_0

### Easter Egg:


![WhatsApp Image 2024-01-21 at 17 34 17](https://github.com/VladRo26/LineFollower/assets/100710098/5255a6b3-b0c0-43f6-9cf8-1826831a6303=200x200)

