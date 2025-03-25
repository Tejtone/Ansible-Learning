<p align="center">
  <img src="https://joshrnoll.com/ansiblelogo.png" width="200" alt="Ansible Logo">
</p>

# Ansible Learning Environment 🐍
To repozytorium zawiera podstawowe konfiguracje Ansible, których używam podczas nauki.  
Środowisko postawione na Proxmox składa się z 13 maszyn wirtualnych:
- **Control Node**: 1 maszyna
- **Webservers**: 4 maszyny
- **Databases**: 3 maszyny
- **Utilities**: 2 maszyny
- **Experimental**: 3 maszyny

## Struktura
- `inventory/`: Pliki z grupami hostów.
- `playbooks/`: Playbooki Ansible do wykonywania różnych zadań.
