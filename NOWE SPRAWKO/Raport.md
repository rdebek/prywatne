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

Wyszukuję podatność:

![](DODATKOWE.PNG)


![](OPJCE.PNG)

Po ustawieniu odpowiednich parametrów i wykonaniu exploita otrzymuję następujący wynik:

![](WYNIKDZIALANIA.PNG)

Co pozwala mi na wykonanie dowolnych komend.

![](wylaczeniezdalne.PNG)

## 3.1 Lista użytkowników SMTP na maszynie vulnix.

Szukam exploitów odnajdujących nazwy użytkowników SMTP:

![](wyszukiwanienazw.PNG)

Przy pomocy *smtp_enum* otrzymuję listę użytkowników:

![](wynikdzialaniaszukaniauzytkownikow.PNG)

## 3.2 Znajdowanie hasła do użytkownika *user* przy pomocy ataku słownikowego:

![](haslodouser.PNG)






