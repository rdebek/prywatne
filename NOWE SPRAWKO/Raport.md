# Raport z testu penetracyjnego.
# Radosław Dębek, nr indeksu: 303689.
## 1. Skanowanie wirtualnych maszyn pod kątem otwartych portów za pomocą **nmap**.

1.1 Host metasploitable:

![](metasploitablenmapscan.PNG)

1.2 Host vulnix:

![](vulnixnmapscan.PNG)

## 1.3. Skanowanie wirtualnych maszyn pod kątem systemu operacyjnego oraz wersji używanych usług.

1.4 Host metasploitable:

![](metasploitableversionscan.PNG)

1.5 Host vulnix:

![](vulnixversionscan.PNG)

## 2. Skanowanie podatności przy pomocy Nessus oraz openVAS.

2.1 Host metasploitable:

![](openvasmetasploitable.PNG)

![](skannessusmetasploitable.PNG)

2.3 Host vulnix:

![](openvasvulnixscan.PNG)

![](nessusvulnixscan.PNG)

# 3. Narzędzie metasploit.

![](ircpodatnosc.PNG)

Jak widać na załączonym obrazku host metasploitable ma podatność UnrealIRCd backdoor. Szukam zatem exploitów ją wykorzystujących przy pomocy metasploit:

![](ustawianieparametrowexploita.PNG)

Po ustawieniu odpowiednich parametrów i wykonaniu exploita otrzymuję następujący wynik:

![](wynikdzialaniaexploita.PNG)

Co pozwala mi na wykonanie dowolnych komend.  
Zdalne wyłączenie maszyny wirtualnej vulnix:

![](wylaczeniezdalne.PNG)

## 3.1 Lista użytkowników SMTP na maszynie vulnix.

Szukam exploitów pozwalających odnalezienie nazw użytkowników SMTP:

![](wyszukiwanienazw.PNG)

Przy pomocy *smtp_enum* otrzymuję listę użytkowników:

![](wynikdzialaniaszukaniauzytkownikow.PNG)

## 3.2 Znajdowanie hasła do użytkownika *user*:

![](haslodouser.PNG)






