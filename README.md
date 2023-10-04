# Appunti di TPSIT.

# JavaScript.

## Funzionamento e controllo dei thread in JavaScript.
### Che cos'è un thread.

In JavaScript, un thread è un singolo flusso di istruzioni all'interno dell'interprete JavaScript, che di default è single-threaded,  il che significa che esegue le istruzioni una dopo l'altra su un singolo thread principale.

## Come vengono gestiti i thread in JavaScript.

Per gestire operazioni asincrone, si utilizzano callback, Promise e async/await. Questi permettono di eseguire operazioni in background senza bloccare il thread principale, consentendo all'interfaccia utente di rimanere responsive. 
I callback sono funzioni passate come argomenti e chiamate quando un'operazione è completata. ** (USATI IN CLASSE) **
Le Promise forniscono un'interfaccia più strutturata per la gestione di operazioni asincrone, mentre async/await semplifica la scrittura di codice asincrono in modo più leggibile.
Nonostante JavaScript non supporti threading multipli nativamente, questi meccanismi consentono di gestire concorrentemente le operazioni e migliorare l'efficienza delle applicazioni web.

## React.

React è una libreria per JavaScript usata per la craezione di UI e per lo sviluppo di WebApp.
React utilizza un approccio basato su componenti, in cui l'interfaccia utente è divisa in piccoli componenti indipendenti, ciascuno dei quali gestisce la propria logica e rendering.

### React jsx.
JSX è un estenzione di React che ci permette di scrivere codice usufruendo di tag come HTML, che ci semplifica di molto la scrittura.
Alcuni esempi:
``` 
const name = "John";
const greeting = <p>Hello, {name}!</p>; 
const element = <h1>Hello, world!</h1>; 
```
## Come installare React

### Lista di comandi per installare React(In Windows powerShell).
Prima installa nodeJS(Dopo ci sta uan descrizione)(Cerca sempre di avere la versione LTS per evitare che durante lo sviluppo possano succedere casini).

```
node -v 
nmp -v
```
^ Usa questi due comandi per visualizzzare la versione di node e npm(Sigla che sta per node packet menager).

```
npm crate vite
```
^ Questo comando serve per scaricare lo strumento vite che in sostanza fa la stessa cosa di webpack(Forse spiegato dopo).
Questo strumento ci permette di usare diversi ambienti noi usiamo React.


Procedimento da terminale(BASH LINUX):
```
@eDalessandr0 ➜ /workspaces/4ci-asynchronous-javascript-eDalessandr0/firstApp (main) $ npm create vite
Need to install the following packages:
create-vite@4.4.1
Ok to proceed? (y) y
✔ Project name: … first-app
✔ Select a framework: › React
✔ Select a variant: › TypeScript

Scaffolding project in /workspaces/4ci-asynchronous-javascript-eDalessandr0/firstApp/first-app...

Done. Now run:

  cd first-app
  npm install
  npm run dev

npm notice 
npm notice New minor version of npm available! 10.1.0 -> 10.2.0
npm notice Changelog: https://github.com/npm/cli/releases/tag/v10.2.0
npm notice Run npm install -g npm@10.2.0 to update!
npm notice 
@eDalessandr0 ➜ /workspaces/4ci-asynchronous-javascript-eDalessandr0/firstApp (main) $ 
```
Alla fine per aprire il nostro progetto seguire i comandi da riga 62 a riga 64.

## NodeJS.

Node è un runtime environment di sviluppo per JavaScript, che ci permette di usare JavaScript come linguaggio come linguaggio dinamico ad esempio py.
Si possono creare anche applicazioni che posso essere fatte andare su computer e server per offrire vari servizi.

## Spin off su file json.
JavaScript Object Notation è un file semplice che gestisce la trasmissone di dati tra server e client.ù
### Caratteristiche di JSON:
Sintassi Semplice: I file JSON utilizzano una sintassi basata su coppie di chiavi e valori.
I dati sono organizzati in oggetti (delimitati da parentesi graffe {}) e in array (delimitati da parentesi quadre []).

Chiavi e Valori: In un oggetto JSON, le chiavi sono stringhe che definiscono il nome di un campo, e i valori possono essere numeri, stringhe, booleani, oggetti, array o null.
### Esempio di JSON 
```
{
  "nome": "Mario",
  "eta": 30,
  "hobby": ["calcio", "musica"],
  "indirizzo":{
    "via": "Via Roma",
    "citta": "Milano"
    }
}
