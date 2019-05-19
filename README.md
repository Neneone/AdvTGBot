# Benvenuto nell'installazione di AdvTGBot!
_Prima di tutto, specifichiamo che per utilizzare AdvancedTGBot bisogna avere una conoscenza almeno minima di PHP_

## Requisiti:
1. Avere PHP7
2. Avere HTTPS Attivo
3. Avere un WebServer

## Installazione:
_Ora procediamo all'installazione di AdvTG! La guida deve essere seguita passo passo._ 
* Creare una cartella ed inserire i file di AdvTG (La cartella deve essere accessibile dal web.)
* Avviare [questo](https://t.me/EasyTGBot) bot e cliccare su "Genera Key"
* Salvare momentaneamente la key in un file.
* Aprire il file index.php nella cartella di AdvTG e modificare la stringa "FPAM" con la key ricevuta dal bot.

## Settare il webhook:
**_A cosa serve il webhook?_**
_Il webhook serve a telegram per comunicarci tutti gli update che il bot deve ricevere_
**_Per settare il webhook dobbiamo fare una richiesta alle API HTTPS di telegram_**
_Ovviamente le {} devono essere rimosse_
* {TOKEN} = Token del nostro bot
* {DOMAIN} = Potrebbe essere anche mattiabl.it
* {DIRECTORY} = directory che conduce alla index.php 
* {KEY} = Key data dal bot che abbiamo salvato in precendeza

https://api.telegram.org/bot{TOKEN}/setwebhook?url=https://{DOMAIN}/{DIRECTORY}/index.php?fpam={KEY}%26token={TOKEN}
Per supporto visita la sezione issues di github

This Source Code Form is subject to the terms of the Mozilla Public
License, v. 2.0. If a copy of the MPL was not distributed with this
file, You can obtain one at http://mozilla.org/MPL/2.0/.
