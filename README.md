# Extra driver for Acer 2-in-1 Laptops, SPIN Series

**Istruzioni per installare i driver del touchpad, touchscreen e penna wacom per i convertibili Acer su Ununtu**

---

- Verificare la distribuzione i uso; questi driver sono stati testati solo per Ubuntu (20.04.4 LTS), potrebbero non finzionare su altre distibuzioni.
  
- È necessario avere almeno 10MB di spazio libero sul disco e una connesione internet funzionante.
  
- Aprire un terminale (<u>Control+Alt+T</u>) ed eseguire il seguente comando per soddisafare tutte le dipendenze: `sudo apt install xdotool acpi`
  
- Assicurarsi che il contenuto di SuperDriver.zip sia stato estratto in <u>$YOUR_HOME_DIRECTORY</u>, aprire un terminale nella propria cartella home (tasto destro nel vuoto, Apri nel terminale)
  
- Consentire l'esecuzione del file *install.sh* con `chmod u+x install.sh`
  
- Eseguire il file *install.sh* con: `./install.sh`
  
- Seguire le istruzioni nel terminale
  

---

###### Attenzione! Non ci assumiamo nessuna responsabilità in caso di brik, perdita di dati, ecc... procedi a tuo richio e pericolo.

---

Una volta terminata l'installazione il computer verrà riavviato e touchpad, touchscreen e penna wacom funzioneranno correttamente.

---

Driver version: 2.01 for Ubuntu 20.04.4 LTS (Focal Fossa)


FAQ

**1.**

> Perchè il driver per il tasto destro della penna non funziona su Wayland?
> 
> ---
> 
> Per funzionare il driver per il tasto destr della penna Wacom utilizza <u>xinput</u> e <u>xdotool</u>, due tool di sistema che non funzionano (correttamente) so Wayland.

**2.**

> Perchè quando premo il pulsante destro della penna senza toccare lo schermo, il clik viene eseguito comunque?
> 
> ---
> 
> Questa è un opzione gestita dai driver xsetwacom
