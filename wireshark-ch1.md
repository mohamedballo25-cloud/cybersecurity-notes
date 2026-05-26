# Wireshark - Analyse ch1.pcap

## Ce que j'ai appris 
- Wireshark lit les fichiers .pcap
  (captures réseau)
- FTP transmet les credentials en clair = dangereux
- On peut filtrer avec : 
  ftp.request.command
- USER = nom d'utilisateur envoyé en clair
- PASS = mot de pass envoyé en clair

## Commandes wireshark utilisées
- Filtre : ftp
- Filtre : ftp.request.command

## Credentials trouvés
- Username : cdts3500
- Password : cdts3500
- Problème : username = password = faille de sécurité !

## Leçon SOC importante
- FTP est dangereux car tout est en clair
- Un attaquant sur le reseau voit tout 
- Solution moderne : SFTP ou FTPS

## Commande terminal utilisée
- wireshark ch1.pcap &
