# Ethernet - Trame (10 pts)

## Ce que j'ai appris
- Une trame Ethernet contient des données encodées
- Le fichier hexadécimal se décode avec xxd -r -p
- Authorization Basic = encodage Base64
- Base64 se décode avec : echo "code" | base64 -d

## Commandes utilisées
- cat fichier.txt
- cat fichier.txt | tr -d ' \n' | xxd -r -p
- echo "code" | base64 -d

## Flag trouvé
- Usernam:password : confi:dential

## Leçon importante
- Pas besoin de Wireshark si les données sont deja en hexa brut
- Wireshark = fichier .pcap complet
- Terminal = données brutes hexa
