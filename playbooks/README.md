# Playbooks - Ansible Automations

Ten katalog zawiera różne playbooki Ansible, które służą do automatyzacji zadań na maszynach wirtualnych.

## Playbooki w tym katalogu:

### 1. **system_update.yml**
Playbook aktualizujący system oraz czyści pamięć cache w grupie `webservers`.

#### Jak używać:
(Jeśli nie jesteście pewni użycia playbooka czy zadziala lub przerwie w polowie wykonywania pracy warto dodać na końcu komendy przydatny argument --check. Jeśli odpowiedź od systemu będzie ok, to możemy uruchomić normalnie playbooka)
```bash
ansible-playbook system_update.yaml --ask-become-pass --check
