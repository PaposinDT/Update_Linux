# KaliSetup.sh

Uno script Bash per automatizzare l’installazione iniziale degli strumenti essenziali su Kali Linux.

## Descrizione

KaliSetup.sh automatizza le operazioni comuni eseguite dopo una nuova installazione di Kali Linux, incluse:

- Aggiornamento del sistema
- Installazione di pacchetti base e strumenti di pentesting
- Attivazione del servizio SSH
- Installazione del metapacchetto completo `kali-linux-everything`

Lo script è pensato per velocizzare la configurazione iniziale, garantendo una base solida e aggiornata.

## Requisiti

- Kali Linux (ultima versione consigliata)
- Accesso root o sudo
- Connessione internet attiva

## Utilizzo

```bash
git clone https://github.com/PaposinDT/KaliSetup.git
cd KaliSetup
chmod +x KaliSetup.sh
sudo ./KaliSetup.sh
```

Panoramica delle funzionalità
Aggiornamento sistema
apt-get update

apt-get upgrade

apt-get dist-upgrade

apt-get autoremove

Pacchetti installati
Categoria	Pacchetti
Strumenti base	git, curl, wget, vim, unzip, zip, tar, build-essential, net-tools
Rete e analisi	nmap, tcpdump, john, hydra, wireshark, aircrack-ng
Recon e OSINT	amass, theHarvester, sherlock
Exploit & reverse	metasploit-framework, exploitdb, radare2, apktool, jadx
Servizi e sicurezza	openssh-server, ufw, fail2ban, tor, proxychains4
Wireless tools	bettercap, reaver, bully
Firmware	firmware-misc-nonfree
Python	python3, python3-pip, pip upgrade

Servizi
Abilitazione e avvio automatico del servizio SSH

Metapacchetti
Installazione del pacchetto completo: kali-linux-everything

Personalizzazione
Puoi modificare lo script per includere altri strumenti o configurazioni specifiche per il tuo flusso di lavoro.
Le opzioni APT sono centralizzate in una variabile (APT_OPTS) per facilitare eventuali modifiche alla modalità di installazione.

Sicurezza
Lo script abilita SSH ma non configura firewall o altre protezioni di rete avanzate.

L'uso di ufw e fail2ban è consigliato su sistemi esposti.

Disclaimer
Questo script è fornito a scopo puramente educativo e per uso personale. L'autore non è responsabile per eventuali danni derivanti da un uso improprio.

Autore

Riccardo Papa

GitHub: github.com/PaposinDT

Telegram: @PaposinDT

PayPal: paypal.me/ricky2006
