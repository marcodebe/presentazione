# TShark Team

### Incidente Leopardo Company

---

## TL;DR

<br>

Nel pomeriggio del giorno 21 dicembre è stato compromesso l'account di un dipendente
dell'azienda per inviare, ad un soggetto esterno, il file
contenente le informazioni confidenziali relative alla commessa **WireCat**

---

### Descrizione dell'attacco

Tra le 21:41 e le 21:42

dal computer *nospringchicken* abbiamo notato attività anomale; attacco al server di posta: scoperta la password di un utente, 
all'interno di un messaggio di posta l'attaccante trova indicazioni riguardanti la posizione del file
  relativo alla commessa; l'attaccante scarica il documento da uno dei vostri server web; l'attaccante invia il documento riservato via mail ad un indirizzo esterno

---

### Recupero informazioni sull'infrastruttura informatica

L'attaccante ha sfrutatto una configurazione insicura per ottenere informazioni
sui server dell'azienda, tecnicamente: DNS zone transfer 

---

### Attacco al server di posta

- L'attaccante ha trovato la password di un dipendente aziendale tramite un
attacco a dizionario, cioè provando password comuni.
- Un messaggio di posta dell'utente indicava dove sarebbe stato archiviato il
documento relativo alla commessa WireCat: sul sito intranet aziendale

---

### Accesso al sito intranet

![Alt Text](Bad_security.png)

- all'indirizzo indicato nella mail l'attaccante trova l'indicazione
  che il sito è stato spostato ad un altro indirizzo
- l'attaccante tenta quindi di accedere al nuovo indirizzo al quale riesce ad accedere solo dopo aver insertito le credenziali *rubate*

# 

@[1,3-6](Present code found within any repo source file.)
@[8-18](Without ever leaving your slideshow.)
@[19-28](Using GitPitch code-presenting with (optional) annotations.)

---

@title[JavaScript Block]

<p><span class="slide-title">JavaScript Block</span></p>

```javascript
// Include http module.
var http = require("http");

// Create the server. Function passed as parameter
// is called on every request made.
http.createServer(function (request, response) {
  // Attach listener on end event.  This event is
  // called when client sent, awaiting response.
  request.on("end", function () {
    // Write headers to the response.
    // HTTP 200 status, Content-Type text/plain.
    response.writeHead(200, {
      'Content-Type': 'text/plain'
    });
    // Send data and end response.
    response.end('Hello HTTP!');
  });

// Listen on the 8080 port.
}).listen(8080);
```

@[1,2](You can present code inlined within your slide markdown too.)
@[9-17](Displayed using code-syntax highlighting just like your IDE.)
@[19-20](Again, all of this without ever leaving your slideshow.)

---?gist=onetapbeyond/494e0fecaf0d6a2aa2acadfb8eb9d6e8&lang=scala&title=Scala GIST

@[23](You can even present code found within any GitHub GIST.)
@[41-53](GIST source code is beautifully rendered on any slide.)
@[57-62](And code-presenting works seamlessly for GIST too, both online and offline.)

---

## Template Help

- [Code Presenting](https://github.com/gitpitch/gitpitch/wiki/Code-Presenting)
  + [Repo Source](https://github.com/gitpitch/gitpitch/wiki/Code-Delimiter-Slides), [Static Blocks](https://github.com/gitpitch/gitpitch/wiki/Code-Slides), [GIST](https://github.com/gitpitch/gitpitch/wiki/GIST-Slides) 
- [Custom CSS Styling](https://github.com/gitpitch/gitpitch/wiki/Slideshow-Custom-CSS)
- [Slideshow Background Image](https://github.com/gitpitch/gitpitch/wiki/Background-Setting)
- [Slide-specific Background Images](https://github.com/gitpitch/gitpitch/wiki/Image-Slides#background)
- [Custom Logo](https://github.com/gitpitch/gitpitch/wiki/Logo-Setting) [TOC](https://github.com/gitpitch/gitpitch/wiki/Table-of-Contents) [Footnotes](https://github.com/gitpitch/gitpitch/wiki/Footnote-Setting)

---

### Template Versions

- #### [Base Template  @fa[external-link gp-download]](https://gitpitch.com/gitpitch/templates/white)
- #### [Code Maximized @fa[external-link gp-download]](https://gitpitch.com/gitpitch/templates/white?p=codemax)
- #### [Speaker Notes @fa[external-link gp-download]](https://gitpitch.com/gitpitch/templates/white?p=speaker)

---

### Questions?

<br>

@fa[twitter gp-contact](@gitpitch)

@fa[github gp-contact](gitpitch)

@fa[medium gp-contact](@gitpitch)

---?image=assets/image/gitpitch-audience.jpg&opacity=100

@title[Download this Template!]

### <span class="white">Get your presentation started!</span>
### [Download this template @fa[external-link gp-download]](https://gitpitch.com/template/download/white)

