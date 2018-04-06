# Eesrakenduste arendamine 2018k

#### [Lindistatud loengud saadaval SIIT YouTube'is](https://www.youtube.com/playlist?list=PLKRRRfRASlMUB-CgyJJLQ-0N3kRIisOp4)

#### [Vaata kodutööde seisu SIIN](http://minitorn.cs.tlu.ee/~romil/GitHubCourseManager/view.php?org=eesrakenduste-arendamine-2018k&admin=romilrobtsenkov&exclude=kursus,1.ea-loeng,2.ea-loeng,klahvimine,3.ea-loeng)

* **Õpetaja:** Romil Rõbtšenkov, [romilr@tlu.ee](mailto:romilr@tlu.ee)
* **Testserver:** lin2.tlu.ee (html, js), greeny.cs.tlu.ee (ssl)
* **Tunni näited:** [~romil/ea17k](http://minitorn.cs.tlu.ee/~romil/ea2018k)

### Ühendus Greeny'sse

* Windows | [VIDEO](https://youtu.be/kg5NAsRQAJ8)

    * [Tunneli loomise juhend](http://minitorn.tlu.ee/~jaagup/kool/java/kursused/09/veebipr/naited/greenytunnel/greenytunnel.pdf)

* Mac OS | [VIDEO](https://youtu.be/RJc-Gvpn9M4)
```
1. open Terminal app
2. write:

ssh university_username@lin2.tlu.ee -L 5555:greeny.cs.tlu.ee:80

3. then write TLU account password. Now you can access greeny from browser localhost:5555

4. open new tab in Terminal (cmd + t) and write:

ssh university_username@lin2.tlu.ee -L 2222:greeny.cs.tlu.ee:22

5. then write TLU account password

5. open FTP client (CyberDuck, FileZilla, Coda etc.) and connect to greeny via SFTP
    host:     127.0.0.1
    port:     2222
    username: YourGreenyUsername
    password: YourGreenyPassword

6. choose one Terminal tab and connect to greeny via ssh, write:
ssh YourGreenyUsername@greeny.cs.tlu.ee
7. then enter your Greeny username password
    ls             – to view files and folders in current path
    cd folderName - to enter folder
    cd ..          – to exit folder to previous path
```

## Kodused tööd ja projektid

* [1. kodutöö](https://github.com/eesrakenduste-arendamine-2017k/1.ea-kodutoo)
* [2. kodutöö](https://github.com/eesrakenduste-arendamine-2017k/2.ea-kodutoo)
* [3. kodutöö](https://github.com/eesrakenduste-arendamine-2017k/3.ea-kodutoo)
* projekt

### GitHub'i töövoog

1. *Fork*'i ülesande/projekti repositoorium (leiab [https://github.com/eesrakenduste-arendamine-2018k/](https://github.com/eesrakenduste-arendamine-2018k/)).
1. *Clone*'i see repositoorium enda arvutisse/serverisse ja määra repositooriumi URL kuhu edaspidi muudatusi salvestad.
  ```
  git clone https://YOURUSERNAME@github.com/YOURUSERNAME/REPOSITORY.git
  
  nt esimese iseseisva töö puhul:
  git clone https://jukujuurika@github.com/jukujuurikas/1.ea-kodutoo.git
  ```
1. Lisa vajdusel oma nimi ja email repositooriumi omanikuks ([Setting your username](https://help.github.com/articles/setting-your-username-in-git/)). Vajadusel hangi endale privaatne e-post @users.noreply.github.com lõpuga (https://github.com/settings/emails)
  ```
  git config --global user.name "Romil Robtsenkov"
  git config --global user.email romilrobtsenkov@users.noreply.github.com
  ```
1. Muuda faile ülesande lahendamiseks ja *Commit*'i iga olulisem muudatus, kasutades kahte käsku.
  ```
  git add .
  ```
  ```
  git commit -m "Added this functionality to the app"
  ```
1. Veendu, et kogu kood on *Commit*'itud.
  ```
  git status
  ```
1. *Push/sync*'i muudatused GitHub'i.
  ```
  git push origin
  ```
1. [Ava *pull request*](https://help.github.com/articles/creating-a-pull-request) ülesande originaalses repositooriumis. Järgi üleasende esitamise tähtaega
1. Muudatusi ja täiendusi võib *push*'ida repositooriumisse, kuni ette antud  kuupäevani.

Tagasisidet saab otse *pull request*'i millele ootan Sinupoolseid kommentaare/mõtteid/küsimusi. Võid julgselt avada *pull request*'i kohe kui hakkad kodutöö kallal tegelama ja siis kui hätta jääd võid esitada sinna küsimuse. Maini kommentaaris minu kasutajat `@romilrobtsenkov` siis jõuan sellele kiiremini vastata.

### Nõuded

Need rakenduvad ka päris elus!

* Peab järgma "head programmeerimise stiili"
    * Muutujate nimed peavad kirjeldama muutujat ning peavad olema inglise keeles
    * Funktsiooni nimi peab olema "lühike"
    * Optimeeri koodi lugemiseks (real ~80 tähemärki)
    * Projektide jaoks tuleb kasutada objektorienteeritud lähenemist
    * Laenatud koodile tuleb viidata
* Boonuspunktid:
    * Loomingulisus (NB! nõuded peavad olema täidetud)

## Kursus
### 1. loeng

1. Sissejuhatus
    * Veebiprogrammeerimise aine kokkuvõte
    * Arutleme, mis antud kursus endas hõlmab
1. Ajalugu
    * ECMAScript
    * iframe > XMLHttpRequest > AJAX
1. JS kasutusvaldkonnad
    * Lehtede interaktiivseks muutmine ([awwwards](http://www.awwwards.com), [cssdesignawards](http://www.cssdesignawards.com))
    * Võrgu koormuse vähendamine
    * AJAX
    * Vormide valideerimine
    * WebSocket ([Chat](http://socket.io/get-started/chat/))
    * Mängud ja meelelahutus ([threeJS](https://threejs.org))
    * Brauserite lisateegid
1. JS piirangud
    * Andmete kirjutamine serverisse
    * Ligipääs andmebaasidele
    * Ligipääs failisüsteemile
    * Akende sulgemine
    * Lõimtöötlus
    * Ligipääs teistele veebilehtedele
    * Browserite erinevused
1. Turvalisus
   * JS koodile ligipääs
   * `window.opener` näide ([On the security implications of window.opener.location.replace()](https://blog.whatever.io/2015/03/07/on-the-security-implications-of-window-opener-location-replace/) by julio)
1. Tunnis kasutatavad tööriistad
1. Javascript'is programmeerimine, näidisrakenduse loomine
    * muutujad, funktsioonid, aeg, sündmuste kuulamine, dokumendi muutmine
1. [1. kodutöö](https://github.com/eesrakenduste-arendamine-2018k/1.ea-kodutoo)
1. **Kohustuslik järgmiseks korrasks!**
   * **Vaata kuidas ja mis järjekorras JS ning brauser koostööd teevad [What the heck is the event loop anyway?](https://www.youtube.com/watch?v=8aGhZQkoFbQ) by Philip Roberts**
   * **Singleton muster [Learning JavaScript Design Patterns](https://addyosmani.com/resources/essentialjsdesignpatterns/book/) by Addy Osmani**
   
### 2. loeng

1. JS rakenduse ülesehitus (objektorienteeritud kood)
    * JS "use strict" – [w3schools](http://www.w3schools.com/js/js_strict.asp), [ECMAScript 5 Strict Mode](http://ejohn.org/blog/ecmascript-5-strict-mode-json-and-more/)
    
   ```JS
   (function(){
      "use strict";

      // rakenduse sisu

   })();
   ```
    * [näide](http://minitorn.cs.tlu.ee/~romil/singleton-example.js) – kas tunned ära kust lehelt on see pärit? 
    * Kasutame Singleton mustrit (Loe kindlasti mustrite kohta lähemalt [Learning JavaScript Design Patterns](https://addyosmani.com/resources/essentialjsdesignpatterns/book/) by Addy Osmani)
1. **Kohustuslik järgmiseks korrasks!**
    **single-page-application artikli põhjal [Reimagining Single-Page Applications With Progressive Enhancement](https://www.smashingmagazine.com/2015/12/reimagining-single-page-applications-progressive-enhancement/)**

### 2. praktikum

1. Selleks, et jooksutada AJAX päringuid kohalikus masinas on vaja nt Chrome käivitada flag'iga `--allow-file-access-from-files`. Oluline on siinkohal välja tuua, et päringu `status` atribuut on pärinug õnnestumise puhul mitte 200 nagu tavaliselt, vaid hoopis 0.
   * MacOS'il `open /Applications/Google\ Chrome.app --args --allow-file-access-from-files`
   * Windows'il `start Chrome --allow-file-access-from-files`
   
**Kohustuslik järgmiseks loenguks!**
    **Täienda skeemi, lisades juurde kasutaja skoori arvutamine**
    **Loe läbi single-page-application artikli põhjal [Reimagining Single-Page Applications With Progressive Enhancement](https://www.smashingmagazine.com/2015/12/reimagining-single-page-applications-progressive-enhancement/)**
    
### 3-4. loeng
1. JS abil andmete salvestamine
    * [JSON](https://www.w3schools.com/js/js_json_intro.asp) annab meile võimaluse teha objektist stringi ja seda kus iganes salvestada ning programmeerimiskeelte ja lehtede vahel andmeid vahetada. 
    * salvestamine brauseri mällu [localStorage](https://www.w3schools.com/html/html5_webstorage.asp) abil
    * UNIX timestamp JS ja PHP vahel – [stack overflow](http://stackoverflow.com/questions/15593759/timestamp-between-javascript-and-php/20502368#20502368)
1. AJAX
   * [GET](http://stackoverflow.com/a/9713078)
   * [POST](http://stackoverflow.com/a/18995200)
1. Automaatsalvestus kui viimasest sündmusest on teatud aeg möödas
   ```JS
   // after typing init autosave

   let timer // GLOBAL
   const doneTypingInterval = 2500

   if (timer) { clearTimeout(timer) }
   timer = window.setTimeout(function () {

      // TODO check if really changed
      save()

   }, doneTypingInterval)
   ```
1. Selleks, et saada lintimist tööle enda arvutis on vaja:
   * Veendu, et arvutis on [Node.js](https://nodejs.org/en/)
   * Alusta projekti kaustas käsuga `npm init` (tekivad package.json/package-lock.json). Seda on vaja teha ühe korra, edaspidi piisab järgmistest toimingutest.
   * Paigalda projekti kaustas [standard](https://www.npmjs.com/package/standard) ja eslint [eslint](https://www.npmjs.com/package/eslint) käsuga `npm i standard eslint `
   * Selleks, et tekkinud kaust node_modules ei läheks git'i üles, tuleb lisada `.gitignore` fail sisuga `node_modules` 
   * Paigalda VS Code'i extension [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
   * Lisa konfiguratsioonifail projekti juurkausta `.eslintrc`, et ESLint teaks arvestada, et kasutad standard style'i.
   ```JSON
   {
     "env": {
       "browser": true
     },
     "extends": ["standard"]
   }   
   ```
   * VS Code sätetes luba parandamine salvestamisel `"eslint.autoFixOnSave": true,` ja veendu, et tavaline lintimine on väljas `"javascript.validate.enable": false,`
1. Varsti enam oma arvutis ainult teha ei saa ning oleks hea kui asi on üleval kuskil serveris, kus on ka HTTPS, nt greeny. Soovitan kasutada VS Code'i extensionit [sftp](https://marketplace.visualstudio.com/items?itemName=liximomo.sftp). Config võib olla midagi sellist, eeldusel, et greeny port 22 on suunatud localhost 2222'te:
   ```JSON
   {
       "protocol": "sftp",
       "host": "localhost",
       "port": 2222,
       "username": "romil",
       "remotePath": "/home/romil/public_html/klahvimine",
       "uploadOnSave": true,
       "syncMode": "full",
       "ignore": [
           ".vscode",
           ".git",
           ".DS_Store",
           "node_modules"
       ]
   }
   ```
1. PS! Kui tahta midagi väga uhket, võib suunata greeny 443 pordi localhosti 443 porti. Seejärel minna ja lisada hosts faili MacOS'il (/etc/hosts) ja Windowsil (c:\Windows\System32\Drivers\etc\hosts) ning lisada rida `127.0.0.1     greeny.cs.tlu.ee`. Seejärel töötab brauseris aadress https://greeny.cs.tlu.ee 

### 5. loeng / praktikum – Chrome extension

1. Chrome extensioni loomine
   - [Alustamine](https://developer.chrome.com/extensions/getstarted)
1. Abiks extension'i uuendamisel [Extensions Reloader](https://chrome.google.com/webstore/detail/extensions-reloader/fimgfedafeadlieiabdeeaodndnlbhid?hl=en)
1. [3. kodutöö](https://github.com/eesrakenduste-arendamine-2018k/3.ea-kodutoo)


## Materjalid ja tööriistad

### Tunnis kasutatavad rakendused
* [Visual Studio Code](https://code.visualstudio.com/)
* koodi valideerimine [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) / [JavaScript Standard Style](https://github.com/standard/standard)
* debug:
    * [Chrome Developer Tools](https://developer.chrome.com/devtools/index)
        * [Official debugging tutorial](https://developer.chrome.com/extensions/tut_debugging)
        * õpetus [JavaScript Diagnosis](http://www.macwright.org/2015/03/10/javascript-diagnosis.html)
    * [Firefox Developer Edition](https://www.mozilla.org/en-US/firefox/developer/)

### Kohustuslik materjal

Välja toodud tundide loetelu juures vastavalt igale tunnile.

### Soovituslik lugemine

* [Kliendipoolsed veebirakendused](http://www.tlu.ee/~jaagup/skriptkeeled/kliendirakendused.pdf)
* [Google JavaScript Style Guide](https://google.github.io/styleguide/javascriptguide.xml)
* [JavaScript Garden](http://bonsaiden.github.com/JavaScript-Garden/)
* [Mozilla's Introduction to Object-Oriented Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Introduction_to_Object-Oriented_JavaScript)
* [Mozilla Developer Network](https://developer.mozilla.org/en/JavaScript)
* [Learn JavaScript](https://developer.mozilla.org/en-US/learn/javascript)
* [w3schools](http://www.w3schools.com/jsref/default.asp)
* [Front-end Job Interview Questions](https://github.com/h5bp/Front-end-Developer-Interview-Questions)
* [JavaScript Best Practices](http://www.thinkful.com/learn/javascript-best-practices-1/)
* [JavaScript Patterns](http://shichuan.github.io/javascript-patterns/)
* [Learning Advanced JavaScript slides](http://ejohn.org/apps/learn/)
* [The JavaScript Interpreter, Interpreted](http://www.slideshare.net/marthakelly/js-interpreter-interpreted) [(video)](https://www.youtube.com/watch?v=iSxNCYcPAFk)
* [Classical Inheritance in JavaScript](http://www.crockford.com/javascript/inheritance.html)
* [Partial Application in JavaScript](http://benalman.com/news/2012/09/partial-application-in-javascript/)
* [Learning JavaScript Design Patterns](http://addyosmani.com/resources/essentialjsdesignpatterns/book/)
* [JS: The Right Way](http://www.jstherightway.org/)
* [Code School](https://www.codeschool.com/paths/javascript)
* [Javascript Trail Map](https://upcase.com/javascript)
* [How To Learn JavaScript Properly](http://javascriptissexy.com/how-to-learn-javascript-properly/)
* [Superhero.js](http://superherojs.com)
* [Teach Yourself to Code](http://teachyourselftocode.com/javascript)

### PHP meeldetuletus
* [PHP Coding Style Guide](http://www.php-fig.org/psr/psr-2/)
* [Veebirakenduste loomine PHP ja MySQLi abil](http://minitorn.tlu.ee/~jaagup/kool/java/loeng/veebipr/veebipr1.pdf)
* [PHP with MySQL Essential Training](http://www.lynda.com/MySQL-tutorials/PHP-MySQL-Essential-Training/119003-2.html)

#### HTML/CSS/JS sandbox'id

* [JS Bin](http://jsbin.com/)
* [CodePen](http://codepen.io/pen/)
* [JSFiddle](http://jsfiddle.net/)

### Git
* [Become a git guru.](https://www.atlassian.com/git/tutorials/)

## Litsents
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />Käesolev <span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" rel="dct:type">leht</span> ja kõik teised https://github.com/eesrakenduste-arendamine-2018k materjalid on <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International Litsensiga</a>.
