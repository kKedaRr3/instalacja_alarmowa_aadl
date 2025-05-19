# instalacja_alarmowa_aadl

## Dane Autorów
Radosław Barszczak
<br>rbarszczak@student.agh.edu.pl


## Opis ogólny
Modelowany system to instalacja alarmowa wykrywania i przeciwdziałania pożarom, zaprojektowana w języku AADL. Celem modelu jest odwzorowanie architektury systemu wczesnego reagowania na potencjalne zagrożenia pożarowe w budynku.
<br><br>System składa się z zestawu czujników i urządzeń wykonawczych, które współpracują w czasie rzeczywistym, aby zapewnić:
- Wczesne wykrycie symptomów pożaru (np. wzrost temperatury, obecność dymu lub czadu),
- Monitoring wizyjny newralgicznych obszarów,
- Automatyczną reakcję w postaci aktywacji zraszaczy przeciwpożarowych,
- Ewentualną sygnalizację alarmową.

## Spis komponentów AADL

### Urządzenia (Devices)
- Czujniki temperatury - służy do pomiaru temperatury w pomieszczeniach 
- Zraszacze przeciwpożarowe - służą do gaszenia pożarów gdy juz takie wystąpią
- Czujniki dymu i czadu - sprawdzają ilość trującego gazu (czadu) i dymu w pomieszczeniu
- Kamera monitorująca - monitoruje newralgiczne miejsca w budynku (serwerownie, kuchnie, rozdzielnie elektryczne)
- Głośniki - informują ludzi o pożarze w budynku
- Lampy alarmowe - podobnie jak głośniki informują w sposób wizualny o pożarze

### Wątki (Threads)

- Wątek zbierający dane z czujników
- Wątek przetwarzający dane
- Wątek wynokujący akcje przeciwpożarowe

### Procesy (Procceses)

- Proces sterujący wszystkimi danymi wchodzącymi i wychodzącymi wewnatrz którego znajdują sie wszystkie powyższe wątki.
  
### Procesor (Proccesor)

- AMD Ryzen 5600h

### Magistrala (Bus)

- Ethernet



