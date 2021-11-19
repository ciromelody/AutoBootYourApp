# AutoBootYourApp
riavvio di se stessa 
E' necessario questo permesso in manifest.xml: uses-permission android:name="android.permission.RECEIVE_BOOT_COMPLETED" 
Creare un receiver broadcast per intercettare il messaggio broadcast :Intent.ACTION_BOOT_COMPLETED
il receiver deve essere strutturato come nel Manifest.
Per versioni superiori o uguali alla versione Q incapsulare l'intent in un pendingintent e creare un allarme di tot secondi
In impostazioni del telefono autorizzare l'app all riavvio
Se si hanno più app che ripartono al riavvio cambiare i secondi dell allarme
Una volta partita l'applicazione è possibile lanciare la tua App preferita da MainActivity 
