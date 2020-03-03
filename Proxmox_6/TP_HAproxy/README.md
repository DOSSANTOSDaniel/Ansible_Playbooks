# TP HAproxy
1- mise à jour du serveur Proxmox
  * pveam update
---
2- Téléchargement des templates sur Proxmox
  * debian-9-turnkey-nextcloud_15.2-1_amd64.tar.gz
  * debian-9-turnkey-dokuwiki_15.1-1_amd64.tar.gz
  * debian-10.0-standard_10.0-1_amd64.tar.gz
  
3- Installation de proxmoxer sur le serveur Proxmox
  * apt install python-pip
  * pip install proxmoxer
  
4- Récupérer les fichiers de configuration de HAproxy et certifications
  * Dans /Ansible_Playbooks/Proxmox_6/TP_HAproxy/files/

5- Exécuter le playbook containers.yml
  * ansible-playbook -i inventory.ini containers.yml
  
6- Exécuter le playbook haproxy.yml
  * ansible-playbook -i inventory.ini haproxy.yml
