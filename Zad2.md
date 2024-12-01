### Sprawozdanie wykonania zadanie 2 - Mikołaj Zawada - 336451

**Transkrypcja mowy z pliku audio**

W celu wykonania zadania na portalu Azure tworzę zasób Speech Services. 

<img width="792" alt="Screenshot 2024-12-01 at 10 24 40" src="https://github.com/user-attachments/assets/a7b13582-5c56-4cc2-ae2a-09e9e0775613">

Klikam utwórz i zasób jest deployowany 

<img width="706" alt="Screenshot 2024-12-01 at 10 26 01" src="https://github.com/user-attachments/assets/877b9b75-e9e9-4016-8990-bbf1add570f7">

Za pomocą komendy dotner new console tworzę nowy projekt .NET na moim komputerze. 

<img width="1070" alt="Screenshot 2024-12-01 at 11 39 05" src="https://github.com/user-attachments/assets/9ea6b05a-f373-4fdc-bb1c-8390e4a656a2">

Dodaję pakiet Azure Cognitive Speech SDK

<img width="1316" alt="Screenshot 2024-12-01 at 11 42 42" src="https://github.com/user-attachments/assets/553c25e2-6ef0-4cd5-a2eb-80bb5d04c825">

Stworzyłem program rozwiązujący problem zadania który działa następująco: 

1. Należy podąc ścieżkę do pliku
<img width="520" alt="Screenshot 2024-12-01 at 14 31 08" src="https://github.com/user-attachments/assets/85ecb557-7b6d-440c-a9fb-2362327a659a">

   
2. Należy podać kod języka
<img width="637" alt="Screenshot 2024-12-01 at 14 31 17" src="https://github.com/user-attachments/assets/73921c0d-f36a-4e0e-b982-2ff030307317">

3. Konfiguracja serwisu
   
<img width="448" alt="Screenshot 2024-12-01 at 14 31 56" src="https://github.com/user-attachments/assets/6079db30-68e0-454a-ae02-d93d01b4c140">

4. Robienie zapytania do stworzonego wcześniej serwisu

<img width="698" alt="Screenshot 2024-12-01 at 14 32 29" src="https://github.com/user-attachments/assets/dc4d61cd-b60d-47fa-ab3d-00f5766f27c8">


5. Odczytywanie odpowiedzi

<img width="561" alt="Screenshot 2024-12-01 at 14 32 40" src="https://github.com/user-attachments/assets/25d8b973-ae61-441d-bfa9-c624763e8840">


Stworzyłem sample za pomocą dyktafonu w telefonie po polsku i po angielsku. Ponieważ mój telefon zapisuje nagrania jako pliki .m4a przy wykorzystaniu ffmpeg konwertuje je na .wav

<img width="1496" alt="Screenshot 2024-12-01 at 14 07 01" src="https://github.com/user-attachments/assets/ce97676c-b761-4a33-910c-80bf3cce38ff">

Wynik działania programu w nagraniu po polsku(Wynik poprawny): 

<img width="528" alt="Screenshot 2024-12-01 at 14 33 05" src="https://github.com/user-attachments/assets/2ee4315b-0a31-444b-8eb0-f57b56076cc2">

Wynik działania programu po Angielsku(wynik poprawny):

<img width="529" alt="Screenshot 2024-12-01 at 14 35 00" src="https://github.com/user-attachments/assets/6cec1170-2217-45de-908a-d8ab2a6eb0a4">
