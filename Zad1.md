
Mikołaj Zawada

Sprawozdanie – Zad 1

Stworzyłem konto na Azure. Stworzyłem nową bazę danych MySQL.

<img width="1048" alt="IMG1" src="https://github.com/user-attachments/assets/b0250b6a-aacb-458a-a49c-d2821c893e06">

W celu połączenia się za pomocą SSMS do serwera należy ustawić opcję połączeń publicznych. Azure automatycznie wybiera IP komputera. Po ustawieniu wypełniamy dane i łączę się za pomocą Microsoft Entra MFA.  
<br/>im2

Im3

Następnie połączyłem się za pomocą Azure Data Studio. Podobnie do SSMS wykorzystałem Microsoft Entra – MFA do autoryzacji.

Im4

Za pomocą połączenia poprzez SSMS wypełniłem bazę 3 rekordami.

Następnie stworzyłem aplikację .NET i dzięki wykorzystanemu connection string:

Im5

Pobieram dane w następujący sposób

Im6

Efekt:

Im7

Następnie stworzyłem wirtualną maszynę w Azure wykorzystując obraz B2s z resztą ustawień domyślną - WarsawIsNice12!

Nawiązałem połączenie za pomocą pliku .rdp

Im8

Pobrałem SQL Server

Im9

Ustawiłem TCP/Ip na enabled oraz port TCP na 1433

Im10

Im11

Oraz dodałem regułę w Firewall pozwalającą SQL Server na korzystanie z portu 1433

Im12

Następnie stworzyłem StorageAccount

Im13

Stworzyłem tabelę products

Im14

Za pomocą Azure Storage Explorer wypełniłem tabelę danymi

Im15

Następnie napisałem aplikację w .NET która łączy się z moim serwisem i pobiera dane z tabelki.  
<br/>im16

Wynik działania programu:  
<br/>im17

**Następnie skonfigurowałem Firewall Azure SQL Database**

Ten etap został wykonany już wcześniej w celu połączenia SSMS do bazy.

Następnie zabrałem się za wprowadzenie do Azure Cosmos DB

Im18

Dodaję nowe elementy do bazy:

Im19

Pobieram dane:

Im20

W zakładce Scale & Settings mogę zmieniać liczbę przetwarzania żądań

Im21

W zakładce monitoring możemy śledzić wykorzystanie bazy

Im22

Napisałem proty program w C# łączący się z bazą i wykonujący operacje CRUD.

CREATE

Im23

READ

Im24

UPDATE

Im25

DELETE

Im26

Efekt działania programu

Im27
