In dieser Aufgabe geht es darum die Befehle zu widerholen welche gebraucht werden um auf dem CA einen Peer zu registrieren.

Tipps:
- docker ps --format "table {{.ID}}\t{{.Names}}\t{{.Command}}" //Befehl um alle Docker Container aufzulisten
- docker exec -it ca.org1.example.com bash //connecten auf container
- fabric-ca-client & fabric-ca-server

1. CA initialisieren und anschliessend starten (mit Benutzer caServerAdmin, passwort AdminsRock)
2. eine CA Admin Identität enrollen
3. Identität Organization1 registrieren & enrollen (name Org1Administrator, secret Org1Rocks, MSP-Pfad $FABRIC_CA_HOME/msp/Org1Administrator)
4. Identität Peer1 registrieren und enrollen (name peer1, secret IAMAPEER, MSP-Pfad $FABRIC_CA_HOME/msp/peer1)

