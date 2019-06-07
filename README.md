# mobile

Questo repository contiene i sorgenti della app ibrida per Android OS.

### Development

1. Clonare il repository `git clone https://github.com/dsirpc/mobile.git`
2. Entrare nella cartella `cd mobile`
3. Il contenuto del codice sorgente del frontend sviluppato in Angular deve essere importato come _submodule_ e sara presente nella cartella `src`. 
Sono state effettuate delle modifiche per adattare il funzionamento con CordovaJS e queste sono contenute nel branch [`android`](https://github.com/dsirpc/frontend/tree/android).
Per popolare la cartella con il sorgente lanciare il comando `git submodule init && git submodule update`
4. Per essere sicuri di aver clonato il branch giusto del submodule è possibile `cd src && git checkout android`
5. È necessario scaricare con `npm` le varie dipendenze. Per Cordova `npm install` dalla root del progetto ed anche per Angular `cd src && npm install`
6. Build: prima di tutto entrare nella cartella con i sorgenti Angular `cd src` e poi `ng build` a questo punto in `../www/` troverete la build del frontend adattata per Cordova
