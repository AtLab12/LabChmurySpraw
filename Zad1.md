
Mikołaj Zawada

Sprawozdanie – Zad 1

Stworzyłem konto na Azure. Stworzyłem nową bazę danych MySQL.

<img width="1048" alt="IMG1" src="https://github.com/user-attachments/assets/b0250b6a-aacb-458a-a49c-d2821c893e06">

W celu połączenia się za pomocą SSMS do serwera należy ustawić opcję połączeń publicznych. Azure automatycznie wybiera IP komputera. Po ustawieniu wypełniamy dane i łączę się za pomocą Microsoft Entra MFA.  
<br/>

<img width="548" alt="IMG2" src="https://github.com/user-attachments/assets/07682f21-3d18-42b9-a9eb-ad7a62a9ce95">
<img width="896" alt="IMG3" src="https://github.com/user-attachments/assets/49f58e68-5960-459e-a6c2-2176f068bd33">


Następnie połączyłem się za pomocą Azure Data Studio. Podobnie do SSMS wykorzystałem Microsoft Entra – MFA do autoryzacji.

<img width="837" alt="IMG4" src="https://github.com/user-attachments/assets/5034a8c5-0fd4-4df3-b35d-958f14027d24">

Za pomocą połączenia poprzez SSMS wypełniłem bazę 3 rekordami.

Następnie stworzyłem aplikację .NET i dzięki wykorzystanemu connection string:

<img width="1040" alt="IMG5" src="https://github.com/user-attachments/assets/ccb6b4ba-bbc0-4223-a820-63684921c0e9">

Pobieram dane w następujący sposób

<img width="1044" alt="IMG6" src="https://github.com/user-attachments/assets/24aa9850-4970-42a3-9a14-b1f752d8522c">

Efekt:

<img width="1040" alt="IMG7" src="https://github.com/user-attachments/assets/bba432d1-4649-4710-8ddc-0a7856029cd8">

Następnie stworzyłem wirtualną maszynę w Azure wykorzystując obraz B2s z resztą ustawień domyślną - WarsawIsNice12!

Nawiązałem połączenie za pomocą pliku .rdp

<img width="1040" alt="IMG8" src="https://github.com/user-attachments/assets/c24c6f8e-2bb3-4981-a8d4-a54836eab31c">


Pobrałem SQL Server

<img width="1040" alt="IMG9" src="https://github.com/user-attachments/assets/ff6f4630-1a4c-450e-99f0-b59cac00ede3">


Ustawiłem TCP/Ip na enabled oraz port TCP na 1433

<img width="1034" alt="IMG10" src="https://github.com/user-attachments/assets/a5d7b73f-8310-4260-be10-609437741280">
<img width="696" alt="IMG11" src="https://github.com/user-attachments/assets/078d3488-576f-4473-80c1-e58eb8452e94">


Oraz dodałem regułę w Firewall pozwalającą SQL Server na korzystanie z portu 1433

<img width="1037" alt="IMG12" src="https://github.com/user-attachments/assets/431b546a-1251-4ef4-916f-8b05a6d95a80">

Następnie stworzyłem StorageAccount

<img width="1059" alt="IMG13" src="https://github.com/user-attachments/assets/d641383f-a4e0-43ef-9636-45dae0220a57">


Stworzyłem tabelę products

<img width="1049" alt="IMG15" src="https://github.com/user-attachments/assets/39674d76-af99-4c1e-b75e-d50a2c0f80c6">


Za pomocą Azure Storage Explorer wypełniłem tabelę danymi

<img width="1036" alt="IMG16" src="https://github.com/user-attachments/assets/47e83451-f11a-468a-a6be-a5e5460383ad">


Następnie napisałem aplikację w .NET która łączy się z moim serwisem i pobiera dane z tabelki.  
<br/>

<img width="1035" alt="IMG17" src="https://github.com/user-attachments/assets/db70f67d-9b55-4ec5-be73-6f053f208df4">

Wynik działania programu:  
<br/>
<img width="1036" alt="IMG18" src="https://github.com/user-attachments/assets/a733125a-709d-4583-8670-c149b1e6b214">


**Następnie skonfigurowałem Firewall Azure SQL Database**

Ten etap został wykonany już wcześniej w celu połączenia SSMS do bazy.

Następnie zabrałem się za wprowadzenie do Azure Cosmos DB

<img width="681" alt="IMG19" src="https://github.com/user-attachments/assets/07384294-6028-43f7-b1fd-35643d48a1ba">


Dodaję nowe elementy do bazy:

<img width="1042" alt="IMG20" src="https://github.com/user-attachments/assets/51de12e2-4611-4086-b571-e921cd2fc316">


Pobieram dane:

<img width="1055" alt="IMG21" src="https://github.com/user-attachments/assets/bff77832-6894-4123-980b-ef7f22d36220">


W zakładce Scale & Settings mogę zmieniać liczbę przetwarzania żądań

<img width="1048" alt="IMG22" src="https://github.com/user-attachments/assets/0397e8c2-4a18-4d96-8da3-69c44fb063a3">


W zakładce monitoring możemy śledzić wykorzystanie bazy

<img width="1010" alt="IMG23" src="https://github.com/user-attachments/assets/342a9ed6-5344-4d27-aea3-4f74b6301457">


Napisałem proty program w C# łączący się z bazą i wykonujący operacje CRUD.

CREATE

<img width="1032" alt="IMG24" src="https://github.com/user-attachments/assets/c0c55510-75d7-4df7-b8da-2b22323b1435">


READ

<img width="1034" alt="IMG25" src="https://github.com/user-attachments/assets/d236605f-505e-4884-90c2-fa27428ea989">


UPDATE

<img width="1032" alt="IMG26" src="https://github.com/user-attachments/assets/d6faa875-0a2d-447f-a205-7e5347843f91">


DELETE

<img width="1036" alt="IMG27" src="https://github.com/user-attachments/assets/05477177-989d-4c23-91ea-1aaf194eb39b">


Efekt działania programu

<img width="1039" alt="IMG28" src="https://github.com/user-attachments/assets/e3850089-9f17-40ea-8f9d-f8781c569efd">
