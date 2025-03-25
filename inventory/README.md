# Inventory - Ansible Hosts Configuration

To repozytorium zawiera plik konfiguracyjny `hosts.ini` z przypisanymi adresami IP dla różnych grup maszyn. Ten plik jest używany przez Ansible do definiowania środowiska, na którym będą wykonywane zadania.

## Struktura pliku `hosts.ini`

Plik `hosts.ini` zawiera następujące grupy maszyn:

### 1. Webservers
Grupa serwerów odpowiedzialnych za aplikacje internetowe.

### 2. Databases
Grupa serwerów odpowiedzialnych za bazy danych.

### 3. Utilities
Grupa serwerów służących do zadań pomocniczych (np. monitoring, logowanie, narzędzia administracyjne).

### 4. Experimental
Grupa maszyn do testów i eksperymentów.

## Użycie pliku `hosts.ini`

Plik `hosts.ini` jest używany przez Ansible do zarządzania maszynami wirtualnymi. W każdym playbooku Ansible, do którego odnosisz się do tego pliku, będziesz wskazywał odpowiednią grupę lub hosta. 

## Po dodaniu adresów IP dla różnych grup musimy w Control Node
wygenerować klucz SSH
``` bash
ssh-keygen -t rsa -b 4096
```
a następnie musimy skopiować klucz SSH na maszyny docelowe
``` bash
ssh-copy-id user@x.x.x.x
```
## Warto dla pewności sprawdzić połączenie pomiędzy systemami
``` bash
ansible all -m ping
```
