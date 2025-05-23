# instalacja_alarmowa_aadl

## Dane Autorów
Radosław Barszczak
<br>rbarszczak@student.agh.edu.pl


## Opis ogólny
Modelowany system to instalacja alarmowa wykrywania i przeciwdziałania pożarom, zaprojektowana w języku AADL. Celem modelu jest odwzorowanie architektury systemu wczesnego reagowania na potencjalne zagrożenia pożarowe w budynku i ewentualne wezwanie służb ratunkowych.
<br><br>System składa się z zestawu czujników i urządzeń wykonawczych, które współpracują w czasie rzeczywistym, aby zapewnić:
- Wczesne wykrycie symptomów pożaru (np. wzrost temperatury, obecność dymu lub czadu),
- Monitoring wizyjny newralgicznych obszarów,
- Automatyczną reakcję w postaci aktywacji zraszaczy przeciwpożarowych,
- Ewentualną sygnalizację alarmową,
- Ewentualne wezwanie służb ratunkowych.

## Spis komponentów AADL

### Urządzenia (Devices)
- Czujniki temperatury - służy do pomiaru temperatury w pomieszczeniach 
- Zraszacze przeciwpożarowe - służą do gaszenia pożarów gdy już takie wystąpią
- Czujniki dymu i czadu - sprawdzają ilość trującego gazu (czadu) i dymu w pomieszczeniu
- Kamera monitorująca - monitoruje newralgiczne miejsca w budynku (serwerownie, kuchnie, rozdzielnie elektryczne)
- Głośniki - informują ludzi o pożarze w budynku
- Lampy alarmowe - podobnie jak głośniki informują w sposób wizualny o pożarze
- Urządzenia wzywające pomoc - w przypadku wystąpienia pożaru straż pożarna jest wzywana na miejsce.

### Wątki (Threads)

- Wątek zbierający dane z czujników dymu i temperatury
- Wątek zbierający dane z kamey
- Wątek podejmujący decyzję na podstawie danych z czujników
- Wątek wykonujący akcje przeciwpożarowe
- Wątek sterujący zawiadamianiem służb ratunkowych

### Procesy (Processes)

- Proces zbierający dane i podejmujący decyzję na podstawie tych danych
- Proces wykonujacy wszystkie działania antypożarowe.
  
### Procesor (Processor)

- AMD Ryzen 5600h

### Magistrala (Bus)

- Ethernet

### System

- System lączący wszystkie komponenty

