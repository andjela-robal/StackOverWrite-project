# O ovom projektu
Projekat StackOverWrite je realizovan kao grupni seminarski rad na fakultetu. Aplikacija je izrađena na osnovu poznatog sajta [Stack Overflow](https://stackoverflow.com) i predstavlja njegovu pojednostavljenu verziju,
namenjenu demonstraciji osnovnih funkcionalnosti sistema za razmenu pitanja i odgovora između korisnika. 
## Funkcionalnosti

Korisniku su pružene sledeće mogućnosti:
- Registracija
- Prijava
- Pregled svih pitanja i odgovora
- Sortiranje pitanja na osnovu tagova
- Postavljanje novog pitanja
- Pregled postojećeg pitanja i svih odgovora
- Postavljanje novog odgovora

## Korišćene tehnologije i alati

- MySQL sistem za rukovanje bazom podataka
- SQL Server Management Studio za administraciju baze podataka
- Programski jezik C#
- Razvojno okruženje Visual Studio
  
# Korisničko uputstvo

### Potrebno za pokretanje
- Instalirati SQL Server
- Instalirati SQL Server Management Studio

### Instalacija
1. Kloniranti ovaj repozitorijum

  `git clone https://github.com/andjela-robal/StackOverWrite-project.git`

2. Kreirati novu bazu podataka pod imenom `stackoverwrite` u SQL Server Management Studio

3. Pokrenuti SQL skripte koje se nalaze u fajlu `stackoverwrite.sql`. Pojedinačne skripte za svaku tabelu se nalaze u folderu `\sql`

4. Po potrebi promeniti ime SQL Servera u konekcionom string-u u `App.config`

   ```
   <connectionStrings>
        <add name="ConDB" connectionString="Data Source=MINWNPC\SQLEXPRESS;Initial Catalog=stackoverwrite;Integrated Security=True" providerName="System.Data.SqlClient"  />
    </connectionStrings>
   ```
5. Pokrenuti (Build) projekat u okviru Visual Studia
