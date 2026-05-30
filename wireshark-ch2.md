# Wireshark - Analyse ch2.pcap

## Ce que j'ai appris
- ch2.pcap contient du trafic TELNET
- TELNET transmet tout en clair = Dangereux
- TELNET envoie chaque caractère séparement
- Follow TCP Stream = voir toute la conversation

## Comment j'ai trouvé les credentials
1. Ouvrir ch2.pcap dans Wireshark
2. Filtrer avec telnet
3. Clique droit sur un paquet
4. Follow => TPC stream
5. Lire les credentials en clair

## Credentials trouvés 
- login : fake
- Password : user

## Leçon SOC importante
- TELNET = tout en clair = Dangereux 
- SSH = chiffré = Sécurisé
- Un attaquant voit chaque caractère tapé ! 

## Commande terminal utilisée
- wireshark ch2.pcap &
