# act1

```
SceneSetup.act1();
```

(...300)

n: E QUESTA É L'ANSIA DELL'UMANA

n: *TU* SEI L'ANSIA 

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Oh hey! Siamo tornati qua? 

`hong({eyes:"0_neutral"})`

n: IL TUO LAVORO É PROTEGGERE L'UMANA DAL *PERICOLO*

`bb({eyes:"look", mouth:"small_lock"})`

n: SOLO RIGIOCANDO QUESTO GIOCO LA STAI METTENDO IN *PERICOLO* ADESSO

n: VELOCE, AVVERTILA!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Umana! Ascoltami, siamo in pericolo! Il giocatore...

[...ci torturerà di nuovo!](#act1_replay_torture)

[...non troverà un finale alternativo!](#act1_replay_alternate)

[...otterrà dissonanza ludonarrativa!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Ci farà raggomitolare su noi stessi e piangere!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Ci farà uccidere il tuo telefono per averti dato un attacco di panico!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Ci farà *NON* tirare un pugno al padrone di casa!
{{/if}} 

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Ci farà dare un pugno al solidale anti-cattivi padrone di casa!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Beh almeno questa volta potremmo non saltare dal tet-
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: CI FARÀ SALTARE DAL TETTO.
{{/if}}

`bb({body:"fear"});`

b: CI CAPITERANNO TUTTE QUESTE TERRIBILI COSE E POI NOI--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Va bene, la storia come *insieme* è la stessa, ma ogni capitolo ha due possibili finali, oltre a tutte le opzioni di dialogo diramati-- 

`bb({body:"fear"});`

b: Il giocatore sarà deluso, chiuderà il browser, cancellerà il nostro gioco e noi--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Aspetta cosa?

`bb({eyes:"normal"});`

b: Questa parte della storia spiegava come tu puoi *SCEGLIERE* di costruire una sana collaborazione con la tua paura,

`bb({eyes:"normal_right"});`

b: ma rigiocando il gioco otterrai la stessa storia e ciò implica che le tue *SCELTE* non importano, 

`bb({eyes:"narrow_eyebrow"});`

b: Mostrando perciò una contraddizzione tra il messaggio del gioco e le meccaniche, 

`bb({eyes:"fear"});`

b: Svelando così il tessuto di questo universo narrativo,

`bb({body:"fear"});`

b: E poi noi--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: MORIREMOOOOOOOO
```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: Okay torniamo nel personaggio 

```
Game.clearText();
```

n4: (LASCIA LA *TUA* ANSIA BLAH BLAH BLAH PIÚ SIMILE ALLE TUE *PAURE* BLAH BLAH BLAH SAI COME FUNZIONA)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Oh bene, il mio lupo è tornato. Faaantastico.

`hong({eyes:"0_neutral"})`

n: IL TUO LAVORO È PROTEGGERE LA TUA UMANA DAL *PERICOLO*

`bb({eyes:"look", mouth:"small_lock"})`

n: DI FATTO, QUEL SANDWICH LA STA METTENDO IN *PERICOLO* PROPRIO ADESSO

n: VELOCE, AVVERTILA!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Umana! Ascolta, siamo in pericolo! Il pericolo è...

`bb({body:"squeeze"})`

n4: (FAI GIOCARE LA *TUA* ANSIA! SCEGLI CIÒ CHE È PIÙ SIMILE A QUELLO CHE TI DICE LA *TUA* PAURA)

(#act1_normal_choice)

# act1_normal_choice

[Pranziamo da soli! Di nuovo!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Non siamo produttivi mentre mangiamo!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Quel pane bianco ci fa male!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Non lo sai che la solitudine è associata alla morte prematura tanto quanto fumare 15 sigarette al giorno?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Um, grazie per aver citato le tue fonti ma--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Il che vuol dire che se non usciamo con qualcuno *adesso* noi-

`bb({body:"panic"})`

b: MORIREMOOOOOO

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: HAI USATO *PAURA DI NON ESSERE AMATI*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Tira fuori il tuo computer e lavora subito!

`hong({eyes:"0_annoyed"})`

h: Um, preferirei non sbriciolare sulla tast--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Se non contribuiamo al corpo della società allora siamo un parassita sociale!

b: Il corpo della società andrà dal dottore della società per avere medicine per uccidere i parassiti sociali e noi-- 
```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: MORIREMOOOOOO

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: HAI USATO *PAURA DI ESSERE UNA CATTIVA PERSONA*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Quegli studi sono mai stati accert-

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b:Il grano processato ci farà aumentare la glicemia e dovranno amputarci tutti gli arti e noi--

`bb({body:"panic"})`

b: MORIREMOOOO

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: HAI USATO *PAURA DI ESSERE FERITI*

(#act1b)

# act1b

n: È SUPER EFFICACE

`bb({mouth:"smile", eyes:"smile"});`

b: Vedi, umana? Sono il tuo fedele lupo da guardia!

`bb({body:"pride_talk"});`

b: Fidati del tuo istinto! I tuoi sentimenti sono sempre validi! 

`bb({body:"pride"});`

n: FAI ARRIVARE LA BARRA DELL'ENERGIA DELLA TUA UMANA A ZERO

n: PER PROTEGGERE I LORO BISOGNI FISICI + SOCIALI + MORALI PUOI USARE: 

n: PAURA DI *ESSERE FERITI* #harm#

n: PAURA DI *NON ESSERE AMATI* #alone#

n: E PAURA DI *ESSERE UNA CATTIVA PERSONA* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (CONSIGLIO: SCEGLI LE SCELTE CHE COLPISCONO PERSONALMENTE LE TUE PAURE PIÙ PROFONDE!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: sai forse è il momento di controllare il mio cellulare.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: PROTEGGI LA TUA UMANA

n: DAL MONDO. DAGLI ALTRI. DA SE STESSA.

n: BUONA FORTUNA

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: ROUND 1: *COMBATTI!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Huh. Facebook mi fa vedere che c'è una festa questo weekend.

`bb({eyes:"uncertain"});`

b: Ma quello strambo non organizza una festa *ogni* weekend? 

`bb({eyes:"uncertain_right"});`

b: Che vuoti interiori starà cercando di colmare? Devono essere messi veramente male!

`hong({eyes:"surprise"});`

h: Sono anche stata invitata?

`bb({eyes:"fear", mouth:"normal"});`

b: Beh, allora!

[Di sì o moriremo di solitudine!](#act1c_loner)

[Di no, è pieno di droghe velenose!](#act1c_drugs)

[Ignoralo, renderemmo la festa triste.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: Quindici sigarette al giorno umana! Quindici!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: Nessuno verrà al nostro funerale, butteranno le nostre ceneri nell'oceano, saremo mangiati da una balena, 
{{/if}}

{{if !_.fifteencigs}}
b: e diventeremo CACCA DI BALENA !
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: In pratica sì, dovremmo andare alla festa!
{{/if}}

{{if _.parasite}}
b: Però porta il computer così possiamo lavorare e non essere un parassita sociale. 
{{/if}}

{{if _.whitebread}}
b: Sempre che non servano PANE BIANCO
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: DIO, se ti farà stare zitta va bene.

h: Dirò di sì

{{if _.whalepoop}}
b: Cacca di balena, umana! Cacca di balena!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: o peggio... PANE BIANCO
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Andremo in overdose con così tanta metanfetamina e pane bianco che il nostro corpo sarà troppo grasso per stare nel forno crematorio!
{{/if}}

{{if !_.whitebread}}
b: Saremo così tanto fatti che il becchino si chiederà come il nostro corpo era *già* pre-imbalsamato!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: In più non possiamo andare alla festa, dobbiamo lavorare o saremo un terribile parassita sociale!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: DIO, se ti farà stare zitta va bene.

h: Dirò di no.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Tutto ciò che facciamo è piangere su come la solitudine sia tanto mortale quanto 15 sigarette al giorno.
{{/if}}

{{if _.parasite}}
b:  Tutto ciò che facciamo alle feste è preoccuparci di come dovremmo esser produttivi.
{{/if}}

{{if _.whitebread}}
b: Tutto ciò che facciamo è preoccuparci di come il cibo spazzatura ci ucciderà.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: mi chiedo proprio perché. 

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Quindi andando li faremmo stare male, ma rifiutando  l'invito staranno male comunque!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: L'UNICA COSA CHE FACCIAMO È  FAR STAR MALE LE PERSONE, QUINDI DOVREMMO STARE MALE

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Ugh, se ti farà stare zitta, va bene.

h: Ignorerò l'invito.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: In ogni caso. Facebook è un po' troppo per adesso. Ho bisogno di qualcosa di più tranquillo. 

`hong({eyes:"neutral"});`

h: Che c'è di nuovo su Twitter?

`bb({eyes:"look"});`

[Oh no, guarda che terribile notizia!](#act1d_news)

[Oh no, quel tweet non sarà mica su di *noi*?](#act1d_subtweet)

[Hey, la GIF di un gatto che beve del latte!](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Mio Dio, sembra che il mondo sia andando a rotoli no?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Sembra che il mondo stia finendo, come se tutto stesse morendo e noi fossimo condannati e non ci fosse nulla che possiamo fare a riguardo.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Retweetiamo quella notizia!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: OKay la retweetterò ma fai silenzio!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: Lasciamo stare, diamo un'occhiata a Snapchat.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: È un subtweet! Un piccolo, subdolo subtweet!

`hong({eyes:"annoyed"});`

h: Probabilmente no? 

`bb({eyes:"narrow", mouth:"small"});`

b: e se stessero parlando alle nostre spalle 

h: Non st--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: DI FRONTE ALLE NOSTRE SPALLE 

`hong({eyes:"sad", mouth:"sad"});`

h: Lo dub-

`bb({eyes:"narrow", mouth:"small"});`

b: e *se invece*

h: S--

`bb({eyes:"narrow_eyebrow"});`

b: *se invece*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: o-KAY, proviamo con Snapchat.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Heh sì, è carino, l'ho retweettato, penso ch--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b:  I GATTI NON RIESCONO A DIGERIRE IL LATTE E SIAMO DELLE TERRIBILI PERSONE A GUARDARE ABUSO SUGLI ANIMALI

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: o-KAY, proviamo con Snapchat.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Huh, foto di ieri sera. Quindi è così che sono quelle feste. 

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Oof, sembra troppo affollato per la mia ansia.

h: Forse non avrei dovuto accettare l'invito?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Cambiare idea? Come una cretina?!](#act1e_yes_dontchange)

[Cambiamo idea! Troppo affollato!](#act1e_yes_changetono)

{{if _.subtweet}}
[Ci stavano decisamente parlando alle spalle](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Aspetta, abbiamo retweettato senza controllare le fonti.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Sai che hai una pessima postura?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Loro contavano sulla nostra presenza e ora tradiamo la loro fiducia? Vuoi morire da sola?!

{{if _.fifteencigs}}
b: QUINCIDI. SIGARETTE.
{{/if}}

{{if _.whalepoop}}
b: CACCA. DI. BALENA. 
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Zitta zitta accetteremo l'invito!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Hai mai sentito parlare di fuggi fuggi?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Nel 2003 un nightclub di Rhode Island ha avuto un incendio e per il panico le persone si sono ammassate sulle uscite e così 100 di loro sono bruciate a morte-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: VUOI CHE SUCCEDA A NOI-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: DI' NO DI' NO DI' NO DI' NO DI' NO DI' NO DI' NO DI' N-

```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Stai zitta, zitta! Dirò di no! Dio mio!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... sembra molto divertente..
h: Forse non avrei dovuto rifiutare l'invito?

`bb({mouth:"normal", eyes:"normal"});`

[Cambiare idea? Come una cretina?!](#act1e_no_dontchange)

[Cambiamo idea! Non moriamo soli!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Ci stavano decisamente parlando alle spalle](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Aspetta, abbiamo retweettato senza controllare le fonti.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Sai che hai una pessima postura?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Tutti contavano su di noi!

b: ...Lasciarli soli e permettergli di avere una bella festa senza un orribile e disgustosa {{if _.whitebread}}white-bread-munching{{/if}} mangiapane come te--


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Stai zitta, zitta! Rifiuterò!
(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: La solitudine cronica aumenta i nostri livelli di cortisolo e il rischio di malattie cardiovascolari o ictus!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: QUINDICI. SIGARETTE.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Stai zitta, zitta! Dirò di sì, Dio mio. 

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Tutti i nostri tweet problematici sono venuti a galla!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: Saremo denunciati e cancellati e trascinati con una corda attaccata a un cavallo per tutta la superstrada dell'informazione!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Perché sei così?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Stiamo diffondendo disinformazione! Stiamo distruggendo la fiducia della libertà di stampa!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Noi siamo il motivo per cui il fascismo risorgerà dalle macerie della democrazia!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: Perché sei così?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Vuoi un pretzel come spina dorsale? Smettila di piegarsi sullo schermo?

```
bb({body:"meta"});
```

b: Vale anche per te.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Perché sei così?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... sembra davvero divertente.

h: Forse non avrei dovuto ignorare l'invito?

`bb({mouth:"normal", eyes:"normal"});`

[Continua a ignorarlo, siamo delle gustafeste](#act1e_ignore_continue)

[Di' di sì.](#act1e_ignore_changetoyes)

[Di' di no.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: Però è abbastanza scortese continuare a ignorarli, no?

`bb({eyes:"normal_right"});`

b: Beh le altre persone *ci* ignorano sempre, quindi

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: diciamo che siamo pari.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: Mi... Mi lasci divertire? 

b: Beh, la solitudine può *ucciderci*.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: Troppo affollato. Le folle sono pericolose. 

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Lasciamo stare. Nuova notifica da Tinder. 

`bb({eyes:"uncertain"})`

b: Cosa, quell'app per scappatelle? 

`hong({eyes:"annoyed"})`

h: Non è un app per scappatelle, è un modo per conoscere nuove pers-

`bb({eyes:"narrow"})`

b: È un app per scappatelle. 

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: Oh, un match! Sembra carino!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Perfavore non rovinarmi anc--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: PERICOLO PERICOLO PERICOLO PERICOLO 

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Stiamo venendo *usate* dagli altri.](#act1f_used_by_others)

[Stiamo solo *usando* gli altri.](#act1f_using_others)

[IL TUO MATCH È UN SERIAL KILLER](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Delle scappatelle forse riusciranno a riempire il buco lì sotto, 

b: ma non riempiranno mai il buco...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: *qua*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Il punto è che MORIREMO SOLE.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Pensi che i genitali degli altri siano dei Pokémon da catturare? 

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (pokemon theme song)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ Voglio essere, la più zo^ccol^a...

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ Come nessuno è mai stato...

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ Cosce e ^culo^, seno voluttuoso-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ con ^cazzo^ e palle sudate!

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ PERVE-MON! GOTTA CA-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Il punto è che siamo un maniaco manipolativo. 

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: Ti intrappoleranno in un pozzo e ti obbligheranno a mangiare pane bianco per farti ingrassare in modo da poter vestire la tua pelle come un completo!
{{/if}}

{{if _.parasite}}
b: Ti colpiranno con un timer pomodoro e diranno "AVRESTI DOVUTO ESSERE PIÙ PRODUTTIVO PARASSITA"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Ti strapperanno la carne in coriandoli sanguinanti, trasformeranno le tue interiora in stelle filanti e mescoleranno il tuo sangue in una ciotola di punch!
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Come suona come invito a una festa?!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: sono stanca di questo gioco.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"loneliness will kill us"... {{/if}}
{{if _.parasite}}"we're a society-parasite"... {{/if}}
{{if _.whitebread}}"don't eat that, it'll kill us"... {{/if}}
{{if _.subtweet}}"they're talking behind our back"... {{/if}}
{{if _.badnews}}"the world is burning"... {{/if}}
{{if _.hookuphole}}"we'll die alone"... {{/if}}
{{if _.serialkiller}}"they're a serial killer"... {{/if}}
{{if _.catmilk}}"cats can't digest milk"... {{/if}}
{{if _.pokemon}}a ^crappy^ parody song... {{/if}}

h: io voglio solo vivere la mia vita.

h: voglio solo essere libera da tutto questo...dolore.

`bb({eyes:"look_sad"});`

b: Hey... umana...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Andrà tutto bene. 

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: Come tuo fedele lupo da guardia, terrò sempre un occhio aperto per il pericolo e farò del mio meglio per tenerti al sicuro.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Lo prometto.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Ultima app. Instagram. Vediamo un po'

`hong({eyes:"sad"});`

h: Altre...foto della festa.

`hong({mouth:"sad"});`

h: Tutti sembrano così felici. Liberi dalle preoccupazioni. Liberi dall'ansia.

`hong({mouth:"anger"});`

h: Perché non posso essere come loro? Perché non posso semplicemente essere *normale?*

`bb({eyes:"normal_right"});`

b: Parlando di feste e a proposito dell'invito di questo weekend, ecco la mia decisione FINALE:

`bb({eyes:"normal"});`

[Dovremmo andare.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Non dovremmo andare.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: Noi dovr--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *VAI. A FARE.*

`hong({body:"2_you"});`

h: *IN. ^CULO^*.

(...500)

b: c

(...1500)

`bb({eyes:"wat_2"});`

b: cos?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: Dirò SÌ a quell'invito,

{{if _.act1g=="go"}}
h: NON perché lo vuoi tu, ma perché lo voglio *io*.
{{/if}}

{{if _.act1g=="dont"}}
h: PRECISAMENTE perché non vuoi che io vada.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: Tu NON mi controlli. 

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: Ora lasciami stare mentre mangio questo delizioso panino in santa ^fottuta^ pace. 

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[AHHHH MORIREMO](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH TUTTI CI ODIANO](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH SIAMO PERSONE ORRIBILI](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH MORIREMO AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH TUTTI CI ODIANO AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH SIAMO PERSONE ORRIBILI AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: CONGRATULAZIONI

(...500)

n: HAI EFFICIENTEMENTE PROTETTO I BISOGNI FISICI + SOCIALI + MORALI DELLA TUA UMANA.

n: GIÀ, GUARDA QUANTO TI È GRATA!
(...500)

n: ORA CHE LA SUA ENERGIA È ZERO, PUOI CONTROLLARE DIRETTAMENTE LE SUE AZIONI. 

`bb({mouth:"smile", eyes:"normal"});`

n: SCEGLI LA TUA MOSSA FINALE

`bb({mouth:"small_lock", eyes:"fear"});`

n: *FINISCILA*

[{COMBATTERE: Punisci il tuo telefono pieno di stress!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{FUGGIRE: Raggomitolati in una palla e piangi!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Il telefono ti stava dando un attacco di panico!

`bb({eyes:"anger"})`

b: Zuckerberg e compagnia stanno dirottando la tua salute per soldi capitalistici azzardati! 

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Punisci il tuo telefono! Distruggilo! Uccidilo!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCIDILO UCCID-

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: Il mondo intero è pieno di pericoli!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Fai come un armadillo! Raggomitolati in una palla per autodifesa!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: RAGGOMITOLATI E PIANGI RAGGOMITOLATI E PIANGI  RAGGOMITOLATI E PIANGI  RAGGOMITOLATI E PIA--

(#act1j)

# act1j

`SceneSetup.act1_outro()`
