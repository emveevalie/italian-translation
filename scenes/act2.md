# act2

`SceneSetup.act2();`

{{if _.badnews && !_.factcheck}}
(#act2-preamble-news1)
{{/if}}

{{if _.badnews && _.factcheck}}
(#act2-preamble-news2)
{{/if}}

{{if _.catmilk}}
(#act2-preamble-cat)
{{/if}}

(#act2-preamble-tinder)


# act2-preamble-news1

```
publish("act2",["dee",3]);
```

s: Si ma hai *visto* quella "notizia" riguardo quell'orribile cosa che sta succedendo da qualche parte?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: c-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Odio le notizie. È tutto sensazionalismo e clickbait.

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: b..bella festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Vero, ma loro seguono solo gli incentivi. Il *vero* problema sono le persone che cliccano il clickbait. 

```
publish("act2",["dee",3]);
```

s: Chi mai retweetterebbe una notizia terribile facendo stare male tutti i suoi amici?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, davvero!

(#act2-preamble-end)


# act2-preamble-news2

```
publish("act2",["dee",3]);
```

s: Comunque hai *visto* quella "notizia" virale? 

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: c-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Sì, palesemente fake. Chi mai ci cascherebbe e lo retweetterebbe? 

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: b..bella festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Ma davvero fra. Ma tipo, sai, aprire Google e controllare prima?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, davvero!

(#act2-preamble-end)


# act2-preamble-cat

```
publish("act2",["dee",3]);
```

s: Come stavo dicendo, il Complesso Industriale dei Meme sfrutta i gatti. 

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: c-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Elabora questa tesi. 

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: b... bella festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Beh, ho visto qualcuno retweettare la GIF di un gatto che beveva latte ieri. 

```
publish("act2",["dee",3]);
```

s: Non possono digerire quella ^merda^! Chi mai retweetterebbe degli *abusi sugli animali*?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, davvero!

(#act2-preamble-end)


# act2-preamble-tinder

```
publish("act2",["dee",1]);
```

s: E quindi niente, non hanno mai risposto!

```
publish("act2",["dee",0]);
publish("act2",["party_hong","next"]);
```

h2: c-ciao...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Anche se avete entrambi matchato su Tinder?

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: b..bella festa...

```
publish("act2",["party_hong","next"]);
```

{{if _.serialkiller}}
(#act2-preamble-serialkiller)
{{/if}}

{{if _.hookuphole}}
(#act2-preamble-hookuphole)
{{/if}}

{{if _.pokemon}}
(#act2-preamble-pokemon)
{{/if}}

# act2-preamble-serialkiller

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Sì, non capisco! Pensavano fossi un boh, un *serial killer*? Che paranoici.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, davvero!

(#act2-preamble-end)


# act2-preamble-hookuphole

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Forse pensavano che una scappatella non potesse riempire il buco nel loro cuore?

s: E basta essere puritani! Apri la mente e poi apri le gambe!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, davvero!

(#act2-preamble-end)


# act2-preamble-pokemon

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Guarda non so! Non era così figa, ma sarebbe stato un buon match.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Gotta Catch 'Em All!™

(#act2-preamble-end)


# act2-preamble-end

```
Game.clearText();
publish("act2-out-1");
music(null, {fade:1});
```

(...3000)

```
music('battle', {volume:0.5});
publish("hp_show");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

n: ROUND DUE: *COMBATTI!*

[Oh no ci odiano tutti!](#act2a_social)

[Stavi mica *adocchiando* la rossa?](#act2a_perv)

[Hey, discutiamo del significato della vita.](#act2a_meaning)

# act2a_social

`bb({eyes:"sad"})`

b: Stiamo rovinando il mood della festa ad esser così tristi!

`bb({eyes:"shock", body:"two_up"})`

b: Stiamo uccidendo le vibes! Stiamo commettendo omicidio di vibes di primo grado!

`bb({eyes:"normal", body:"normal"})`

b: Umana, dobbiamo andarcene *ora* prima---

```
_.a2_first_danger = 'social';
_.a2_attack_1 = "alone";
```

(#act2b)

# act2a_perv

`bb({eyes:"suspect"})`

b: Lei è più bella di noi, il che significa che anche solo *guardandola* noi---

`bb({eyes:"shock", body:"two_up"})`

b: SAREMO MANIACI. 
`bb({body:"normal"})`

b: Siamo inquietanti, cattivi, brutti terribili brutti perver-

```
_.a2_first_danger = 'perv';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2a_meaning

`bb({body:"one_up", eyes:"normal_r"})`

b: Alla fine di tutto, cosa possiamo fare che veramente importi? 

`bb({body:"normal", eyes:"sad"})`

b: Contribuire all'umanità? Tutte le grandi opere decadono come quella di Ozymandias. Amare? La morte ci separerà sempre.

`bb({eyes:"sad_r"})`

b: E quanta morte! *Noi* moriremo. I *nostri cari* moriranno.

`bb({eyes:"shock", body:"two_up"})`

b: Cavolo, la Seconda Legge della Termodinamica significa che il nostro *universo* morirà! 

`bb({eyes:"suspect", body:"normal"})`

b: Certo, "la morte ci fa apprezzare la vita?" Sarebbe come dire che la schiavitù è una cosa buona perché ci fa apprezzare la libertà!

`bb({body:"one_up"})`

b: Certo, "devi crearti il tuo significato?" Esattamente ciò che fanno i cultisti e i complottisti! 

`bb({eyes:"shock", body:"two_up"})`

b: La vita non ha significato, la morte non ha significato, nemmeno *significato* ha significato! Cosa dovrebbe fare un anima mort--

```
_.a2_first_danger = 'meaning';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2b

`bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"suspect"})`

b: Um... riesci a sentirmi, umana?

`bb({eyes:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"shock", mouth:"small_talk", body:"chest", MOUTH_LOCK:true})`

b: *SUSSULTO*

`bb({mouth:"small_talk"})`

b: DEVO AVVERTIRTI RIGUARDO A...

[*Altro* sullo stesso pericolo!](#act2b_louder)

{{if _.a2_first_danger=="social"}}
[Un *diverso* pericolo sociale!](#act2b_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[Un *diverso* pericolo morale!](#act2b_different_moral)
{{/if}}

[Stai ignorando il pericolo! È pericoloso!](#act2b_ignore)

# act2b_louder

`_.a2_first_choice = "louder"`

{{if _.a2_first_danger=="social"}}
(#act2b_louder_social)
{{/if}}

{{if _.a2_first_danger=="perv"}}
(#act2b_louder_perv)
{{/if}}

{{if _.a2_first_danger=="meaning"}}
(#act2b_louder_meaning)
{{/if}}

# act2b_louder_social

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: LE EMOZIONI SONO CONTAGIOSE! SE NON TE NE VAI SUBITO INFETTERAI TUTTI CON LE TUE MALATTIE MENTALI!

b: Creerai un epidemia mortale di SINDROME DELLO SFIGATO TRISTE

`bb({eyes:"suspect", body:"normal", mouth:"normal"})`

b: Dobbiamo uscire di qui e metterci in quarantena per sempre in una piccola stanza con Netflix e consegne a domicilio!

```
_.a2_second_danger = 'netflix';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "a quarantine";
```

(#act2c)

# act2b_louder_perv

`bb({eyes:"suspect", body:"two_up", mouth:"normal"})`

b: DON'T BE A CREEP. IT'S AGAINST THE LAW! NON ESSERE UN MANIACO, È CONTRO LA LEGGE!

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: Legge dei Maniaci, Sezione 74.5: (1) Ogni persona che guarda (a) quelle spalle muscolose (b) quel tondo sedere (2) saranno note come 

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: "UN GRANDE E DISGUSTOSO PERVERTITO"

```
_.a2_second_danger = 'law';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "the law";
```

(#act2c)

# act2b_louder_meaning

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: A dirla tutta, anche se trovassi un obbiettivo nobile nella vita, potresti *comunque* rovinare tutto!

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Alfred Nobel voleva la pace mondiale e che le culture potessero capirsi a vicenda, perciò ha deciso di rendere più facile gli spostamenti.

`bb({eyes:"normal_r"})`

b: So he needed a way to cheaply create train tunnels. So he invented a new material called "dynamite"... Aveva bisogno di un modo di creare tunner per i treni economicamente. Quindi ha inventato la "dinamite"...

`bb({body:"one_up", eyes:"normal"})`

b: che è stata poi usata nella prima guerra mondiale per UCCIDERE MILIONI DI PERSONE

`bb({body:"two_up", eyes:"shock"})`

b: È L'EFFETTO FARFALLA, UMANA! QUANTE PERSONE STAI UCCIDENDO ACCIDENTALMENTE ORA-

```
_.a2_second_danger = 'butterfly';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "World War I";
```

(#act2c)

# act2b_different_social

`_.a2_first_choice = "different"`

`bb({eyes:"normal_r", body:"point", mouth:"normal"})`

b: In realtà sai cos'è peggio di non piacere a nessuno? Piacere *a tutti*.

`bb({body:"one_up", eyes:"suspect", mouth:"normal"})`

b: Ovvero, diventare uno di *questi*  animali da festa a caccia di piacere.

`bb({body:"normal", mouth:"small"})`

b: Una vita vuota con amici superficiali che ti conoscono solo superficialmente!

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Umana, dobbiamo scappare da questi zombie del piacere prima che ci facciano diventare come loro!

```
_.a2_second_danger = 'zombies';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "zombies";
```

(#act2c)

# act2b_different_moral

`_.a2_first_choice = "different"`

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Ci sono persone che stanno morendo in genocidi e carestie *proprio adesso* mentre noi facciamo festa!

`bb({body:"point", eyes:"closed", mouth:"small"})`

b: Un saggio una volta disse "l'unica cosa necessaria per il trionfo del male è che i buoni non facciano nulla".

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: NON STIAMO FACENDO NULLA.

`bb({mouth:"small"})`

b: FACENDO FESTA, STIAMO AIUTANDO *HITLER*.

```
_.a2_second_danger = 'hitler';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "Hitler";
```

(#act2c)

# act2b_ignore

`_.a2_first_choice = "ignore"`

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Pensi di essere al sicuro solo perché hai tolto le pile al rilevatore di monossido di carbonio?

`bb({eyes:"suspect_r"})`

b: Non sentirai nemmeno il veleno! Semplicemente ti verrà sonno e tu--

`bb({body:"scream_c_1"})`

b: MORIRAIIIIIII

```
_.a2_second_danger = 'ignore';
_.a2_attack_2 = "harm";
_.a2_hoodie_callback = "carbon monoxide";
```

(#act2c)

# act2c

```
hong({body:"ignore_sweat"});
bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true});
```

b: ...

`bb({eyes:"happy", mouth:"smile", body:"chest"})`

b: Menomale umana, penso tu mi senta di nuovo!

`bb({eyes:"closed", body:"point"})`

b: TI AVVERTIRÒ RIGUARDO...

{{if _.a2_first_choice=="louder"}}
[*Altro ancora* dello stesso pericolo!](#act2c_louder)
{{/if}}

{{if _.a2_first_choice!="louder"}}
[*Altro* dello stesso pericolo!](#act2c_louder)
{{/if}}

{{if _.a2_first_danger=="social"}}
[Un *diverso* pericolo sociale!](#act2c_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[](#act2c_different_moral)
{{/if}}

[Hai controllato il punch prima di berlo?](#act2c_punch)

#act2c_louder

{{if _.a2_second_danger=="netflix"}}
(#act2c_louder_netflix)
{{/if}}

{{if _.a2_second_danger=="law"}}
(#act2c_louder_law)
{{/if}}

{{if _.a2_second_danger=="butterfly"}}
(#act2c_louder_butterfly)
{{/if}}

{{if _.a2_second_danger=="zombies"}}
(#act2c_louder_zombies)
{{/if}}

{{if _.a2_second_danger=="hitler"}}
(#act2c_louder_hitler)
{{/if}}

{{if _.a2_second_danger=="ignore"}}
(#act2c_louder_ignore)
{{/if}}

# act2c_louder_netflix

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: In realtà, Netflix e cibo a domicilio non vanno ancora bene! Infetteremmo il driver! 

`bb({body:"one_up", mouth:"small"})`

b: Dobbiamo trasferirci nel territorio dello Yukon canadese e far sì che il cibo ci sia consegnato da un drone!

`bb({body:"two_up", mouth:"normal"})`

b: E poi dovrebbero sterilizzare il drone per pulirlo dai nostri GERMI DA SFIGATO TRISTE

`_.a2_attack_3 = "alone";`

`_.a2_hoodie_callback = "a quarantine";`

(#act2d)

# act2c_louder_law

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: IL GRANDE E DISGUSTOSO PERVERTITO sarà condannato a 72 ore in una di quelle macchine per l'umiliazione pubblica medievali

b: almeno che non gli *piaccia* segretamente quel tipo di cosa...

`bb({body:"scream_a_1"})`

b: visto che sono UN GRANDE E DISGUSTOSO PERVERTITO

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "the law";`

(#act2d)

# act2c_louder_butterfly

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: EFFETTO FARFALLA! Stai usando un bicchiere di plastica non biodegradabile? 

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: BAM, IN UNA DISCARICA C'È UNA PERDITA DI VELENO E UCCIDE UN BAMBINO 

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: Stai sudando e il tuo cuore batte?

`bb({body:"scream_a_1"})`

b: BAM, MANDI IN BANCAROTTA IL NOSTRO SISTEMA SANITARIO E MUOIONO IN MILIONI

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "the butterfly effect";`

(#act2d)

# act2c_louder_zombies

`bb({body:"normal", mouth:"small", eyes:"angry"})`

b: Questi zombie del piacere barcolleranno verso di te borbottando,

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: LIIIIIKE. TANTI LIIIIIKE.

`bb({body:"scream_a_1"})`

b: Poi ti MORDERANNO e ti trasformeranno in un BRO SENZACERVELLO e/o una P^UTTANA^ SCONSIDERATA!

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "zombies";`

(#act2d)

# act2c_louder_hitler

`bb({body:"scream_a_1"})`

b: I NAZISTI STANNO RIMARCIANDO SULLE STRADE PROPRIO ORA

`bb({body:"one_up", mouth:"smile", eyes:"happy"})`

b: Dicendo, *menomale che quelle "brave persone" hanno poltrito facendo cose tipo "rilassarsi" e "prendersi cura di loro stessi!*

`bb({body:"point", mouth:"smile", eyes:"happy_r"})`

b: *Ora i nostri piani possono proseguire, con lager anticipo!*

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "Hitler";`

(#act2d)

# act2c_louder_ignore

`bb({body:"normal", mouth:"normal", eyes:"normal_r"})`

b: Ma a pensarci bene, come facciamo a sapere se questo edificio *ha* un rilevatore di monossido?! 

`bb({body:"two_up", mouth:"small", eyes:"normal"})`

b: E se tutti stessimo venendo avvelenati *PROPRIO ADESSO?*

`bb({body:"scream_a_1"})`

b: NON VEDREMO NEMMENO LA MORTE AVVICINARSI. SMETTEREMMO SEMPLICEMENTE DI ESISTE PER SEMPRE E SEMPRE E SEM--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "carbon monoxide";`

(#act2d)

# act2c_different_social

`bb({body:"normal", mouth:"normal", eyes:"sad"})`

b: Ma se fossimo *sostanzialmente incapaci* di essere mai amati o di amare qualcun'altro?

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: E se qualcosa si fosse rotto irreversibilmente dentro di noi tanto tempo fa? O se non fosse proprio mai esistito?

`bb({body:"scream_a_1"})`

b: AHH SIAMO ROTTE! ROTTE ROTTE ROTT--

`_.a2_attack_3 = "alone";`

(#act2d)

# act2c_different_moral

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: E se fossimo solo *sostanzialmente marci?*

`bb({body:"one_up", eyes:"sad"})`

b: Gli altri hanno una predisposizione al fare del bene, mentre noi facciamo del "bene" solo per vergogna o sensi di colpa, se lo facciamo.

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: E se fosse nella nostra natura il fare male agli altri? E se non potessimo essere *nulla* oltre che a un peso per i nostri cari? 

`bb({body:"scream_a_1"})`

b: AHH SIAMO ROTTE! ROTTE ROTTE ROTT--

`_.a2_attack_3 = "bad";`

(#act2d)

# act2c_punch

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Non sono irrazionale. Le persone *drogano* il punch. Quella è una cosa vera che succede veramente.

`bb({eyes:"suspect"})`

b: Umana, ti fa male la testsa? Ti senti gli arti flaccidi? Penso che stiamo morendo.

`bb({body:"scream_a_1"})`

b: AHHH STIAMO MORENDO! STIAMO MORENDO STIAMO MORENDO STIAMO MOR--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "punch bowls";`

(#act2d)

# act2d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"attacked"});
attack("20p", _.a2_attack_1);
```

(...401)

```
hong({body:"attacked_2"});
attack("20p", _.a2_attack_2);
```

(...401)

```
hong({body:"attacked_3"});
attack("20p", _.a2_attack_3);
```

(...1001)

h: C^AZZO^!

h: F^OTTUTO^ F^OTTUTISSI^MO *C^AZZOOOO^*

`bb({body:"two_up", mouth:"smile", eyes:"happy"});`

b: Yay, umana! Puoi sentirmi di nuovo, sono felicissima!

`bb({body:"normal", mouth:"small", eyes:"sad"})`

b: Perché mi stavi ignorando?

`hong({body:"facepalm"})`

h: Porca ^puttana^, sei una completa idiota.

`hong({body:"facepalm_2"})`

h: Conosci quella storia dei Nativi Americani?

h: "Ci sono due lupi dentro di te, uno è speranza, l'altro disperazione, che lupo vince? Quello che nutri."

```
hong({body:"facepalm_3"});
bb({eyes:"normal"});
```

h: Stavo cercando di farti morire di fame, sadistica ^stronza^!

`hong({body:"smile", mouth:"smile"})`

h: Al diavolo, proverò con delle affermazioni positive.

h: *Sono amata. Sono buona. Sono intelligente. Sono bella. Sono speciale.*

`bb({eyes:"suspect"});`

[Perbacco, che narcisismo!](#act2d_narcissist)

[Sai che le affermazioni sono state *smentite?*](#act2d_disproven)

[omg non dare crediti agli indigeni per delle storie random](#act2d_racist)

# act2d_disproven

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Difatto hanno l'effetto contrario per persone con bassa autostima!

`bb({body:"one_up", mouth:"small", eyes:"normal"})`

b: Era uno studio ben disegnato – studio randomico e controllato, lo sperimentatore non sapeva chi fosse in quale gruppo.

`bb({body:"two_up", mouth:"small", eyes:"normal_r"})`

b: Risultati: con un autostima bassa, ripetere queste affermazioni ti fa stare *peggio* che se non avessi detto nulla direttamente!

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Wood 2009, Psychological Science. Cercalo su Google Scholar, umana,

`bb({body:"scream_b_1"})`

b: E POI SMETTI DI DIFFONDERE FAKE NEWS NON SCIENTIFICHE

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_narcissist

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Hai *bisogno* di vedere umilmente i tuoi difetti per crescere come persona!

`bb({body:"two_up", eyes:"suspect"})`

b: Non puoi spruzzare deodorante per ambienti in una stanza con la muffa! Nascondere i tuoi difetti ti rende peggiore a lungo termine. 

`bb({body:"chest", mouth:"smile", eyes:"closed"})`

b: Thankfully, I, as your loyal guard-wolf, can alert you to your flaws. And right now, it's- Fortunatamente, io, come tuo fedele lupo da guardia, posso avvertirti dei tuoi difetti. Giusto adesso, 

`bb({body:"scream_b_1"})`

b: SEI SBAGLIATA. COMPLETAMENTE SBAGLIATA. 

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_racist

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: I nativi americani sono *persone reali,* non dei "nobili selvaggi" che puoi tirar fuori per rendere i tuoi consigli da biscotto della fortuna più *esotici*.

`bb({eyes:"suspect_r"})`

b: Stai riducendo individui e culture complesse a biglietti d'auguri! Quello è "razzismo benevolo"!

`bb({body:"scream_b_1"})`

b: SMETTILA DI ESSERE RAZZISTA CRETINA STRABICA 

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2e

h: ^FANCULO^.

`hong({body:"yell", mouth:"yell"})`

h: Sai cosa? Sei *irrazionale*.

h: Tutti sanno che le emozioni sono irrazionali! Specialmente la paura! 

`hong({body:"facepalm_2"})`

h:  Sei un inutile rimasuglio dell'evoluzione, come la mia appendice o i denti del giudizio!

`hong({body:"yell", mouth:"yell"})`

h: ^Dannazione^, questa metafora del lupo è stupida! Siete solo degli stupide neuro-chimiche nella mia testa. 

`hong({body:"cross", mouth:"cross"})`

h: Quindi perché dovrei ascoltare un inutile, irrazionale, inesistente pezza di ^merda^ come te?!

`bb({eyes:"sad", MOUTH_LOCK:true})`

b: ...

[Cavolo, umana. Questo fa male.](#act2e_hurtful)

[Sono un sentimento. I sentimenti sono validi.](#act2e_valid)

[Umana, siamo *entrambe* "solo sostanze chimiche."](#act2e_rational)

# act2e_hurtful

`bb({body:"chest"})`

b: Sono *parte* di te, lo sai. Quando dici cose così, *ti* ferisci.

`bb({body:"scream_a_1"})`

b: Perché ti colpisci, umana? SMETTI DI COLPIRTI. 

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2e_rational

`bb({body:"normal", mouth:"normal", eyes:"normal_r"});`

b: Le tue motivazioni più profonde sono dopamina, le tue gioie più ricche serotina. 

`bb({body:"one_up"});`

b: I tuoi ricordi sono pesi sinaptici, la tua ragione è solo segnali elettrici soggetti a guasti.

`bb({eyes:"normal", body:"normal"});`

b: Quindi se il mio essere "solo sostanza chimica" significa che *io* sono irrazionale... Allora vuol dire che *tu sei* irrazionale!

`bb({body:"two_up", eyes:"shock"});`

b: And if we're *both* irrational, then we'll *never* figure out how to be fulfilled and happy! E se siamo *entrambe* irrazionali, allora non capiremo *mai* come essere felici e soddisfatte!

`bb({body:"scream_a_1"})`

b: AHH SIAMO ROTTE! ROTTE ROTTE ROTTE ROT--

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2f)

# act2e_valid

`bb({body:"normal", mouth:"normal", eyes:"suspect"});`

b: Aspetta... "loro" dicono che i sentimenti sono validi, che dovresti sempre accettare le tue emozioni. 

`bb({eyes:"suspect_r"});`

b: Ma "loro" dicono anche che le emozioni sono irrazionali, che non ci si può fidare.

`bb({eyes:"angry"});`

b: Oh accidenti, "loro" ci stanno mentendo dall'inizio!

`bb({body:"scream_a_1"})`

b: "LORO" CI NUTRONO DI CONTRADDIZIONI PER RENDERCI DIPENDENTI DALL'INDUSTRIA DELL'AUTO-AIUTO

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2f

`hong({body:"defeated", MOUTH_LOCK:true});`

h: ...

h: Odio tutto questo. Dio fa così male *odio* tutto questo. 

h: Non posso accontentarti. Non posso ignorarti. Non posso combatterti. 

`bb({eyes:"suspect"});`

h: Non importa che faccio, non riesco a liberarmi di t--

`bb({body:"cry_1"});`

b: Beh forse NON *DOVRESTI* LIBERARTI DI ME.

`bb({body:"cry_2"});`

b: Come pensi che mi senta *io*, umana?!

`bb({body:"cry_4", mouth:"cry", eyes:"cry"})`

b: Sto facendo del mio meglio per essere il tuo cane da guardia, ma continui a vedermi come il lupo cattivo!

b: Quindi provo *ancora di più* ad avvertirti del pericolo! *Più pericolo*! *Diverso pericolo*

`bb({eyes:"cry_2"})`

b: Ma non importa quanto duramente io provi a proteggerti, tu pensi *ancora* io sia tua nemica!

`bb({body:"cry_5"});`

b: Che sto facendo di sbagliato?!

`bb({body:"cry_2"});`

b: So che faccio schifo. Ma ci sto *provando*, umana! 

`bb({body:"cry_3"});`

b: ...sto provando. 

`bb({body:"cry_6", mouth:"right", eyes:"cry_r_1"});`

b: Non devi dar retta ai miei avvertimenti, darmi ragione, e nemmeno ti devo piacere. 

`bb({eyes:"cry_r_2"});`

b: Io... Tutto ciò che voglio è che tu sia paziente con me. 

`bb({eyes:"cry_r_3"});`

b: Voglio solo che tu stia con me per un po', invece di girarti e--

```
bb({eyes:"cry_r_4"});
hong({body:"listen"});
```

r: Hey.

```
hong({body:"look"});
Game.clearText();
publish("act2-in-2");
publish("hp_hide");
music('party1', {volume:0.4, fade:2});
```

(...2000)

```
publish("act2",["party_hunter",2]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Sembra tu sia intrappolata in una battaglia con te stessa, ragazza. 

```
publish("act2",["party_hunter",3]);
publish("act2",["party_hong",13]);
```

h2: Era così ovvio?

```
publish("act2",["party_hunter",4]);
publish("act2",["party_hong",14]);
```

r: Stavi, uh, borbottando contro la tua felpa {{_.a2_hoodie_callback}} o qualcosa del genere. 

```
publish("act2",["party_hunter",13]);
publish("act2",["party_hong",15]);
sfx("rustle", {volume:0.6});
setTimeout(function(){
	publish("act2",["party_hong",16]);
	sfx("concrete_step3", {volume:0.6});
},401);
setTimeout(function(){
	publish("act2",["party_hong",17]);
	sfx("concrete_step4", {volume:0.6});
},801);
```

h2: oh dio sono un disastro.

```
publish("act2",["party_hunter",7]);
publish("act2",["party_hong",18]);
sfx("squeak");
```

r: Hey. Non sei sola, amica. L'ansia è super comune.

```
publish("act2",["party_hunter",5]);
publish("act2",["party_hong",19]);
```

{{if _.act1_ending=="fight"}}
r:  Diamine, ieri ho sentito che qualcuno del campus ha avuto una crisi isterica e ha distrutto il suo telefono! 
{{/if}}

{{if _.act1_ending=="flight"}}
r: Diamine, ieri ho sentito che qualcuno nel campus si è fatta su in una palla come un armadillo e ha pianto!
{{/if}}

```
publish("act2",["party_hunter",2]);
```

r: Senti: so come ci si sente ad avere un animale nella testa. 

```
publish("act2",["party_hunter",8]);
```

r: *Tutti* lo sappiamo. È per questo che organizzo feste ogni weekend, per dimenticarci delle preoccupazioni e dell'animale. 

```
publish("act2",["party_hunter",9]);
publish("act2",["party_hong",20]);
```

h2: ma la mia ansia...

```
publish("act2",["party_hunter",2]);
publish("act2",["party_hong",21]);
```

r: Tranquilla, ragazza. Ero come te. Ma poi ho trovato un trucco per far star zitta quella voce per sempre...

```
publish("act2",["party_hunter",3]);
Game.clearText();
music(null, {fade:1});
```

(...2001)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",22]);
sfx("rustle");
```

(...2501)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",23]);
sfx("rustle2");
```

(...1001)

```
publish("act2",["party_hunter",11]);
```

r: La mia miscela speciale. È un po' più forte di... Beh, qualsiasi cosa legale in realtà.

```
publish("act2",["party_hunter",12]);
publish("act2",["party_hong",24]);
```

r: Dacci dentro, ^stronza^!

```
hong({body:"hold"});
bb({body:"normal", mouth:"small", eyes:"wat"});
Game.clearText();
Game.WORDS_HEIGHT_BOTTOM = -1;
publish("act2-out-3");
publish("hp_show");
```

(...3500)

[Oh mio Dio.](#act2g_1) `Game.OVERRIDE_CHOICE_LINE=true`

[Questo è un cattivo modo di reagire.](#act2g_2) `Game.OVERRIDE_CHOICE_LINE=true`

[Non accettare drink dagli sconosciuti.](#act2g_3) `Game.OVERRIDE_CHOICE_LINE=true`

# act2g_1

b: O--

(#act2g)

# act2g_2

b: T--

(#act2g)

# act2g_3

b: D--

(#act2g)

# act2g

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"forward", mouth:"forward"});
bb({body:"frazzled", mouth:"frazzled", eyes:"frazzled"});
```

h: Mmm, che palette squisita!

h: Un sapore corposo di "zittisci la tua mente" con un sottile retrogusto di "non sentire mai più nulla"!

b: Male, umana. Molto, molto male. 

[È così che *iniziano* le dipendenze.](#act2h_opt1) `Game.OVERRIDE_CHOICE_LINE=true`

[*Sapevo* che non stava bene!](#act2h_opt3) `Game.OVERRIDE_CHOICE_LINE=true`

[Ah e potrebbero averlo drogato!](#act2h_opt2) `Game.OVERRIDE_CHOICE_LINE=true`


# act2h_opt1

b: È così che *ini*--

(#act2h)

# act2h_opt2

b: Ah e potreb--

(#act2h)

# act2h_opt3

b: *Sapevo* che no--

(#act2h)

# act2h

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"back", mouth:"back"});
bb({body:"panicked", mouth:"panicked", eyes:"panicked"});
```

h: Delizioso *e* meno costoso dello psicologo!

b: UMANA FERMA PERFAVORE

h: Hehehe!

h: Cos'hai intenzione di fare a riguardo, ^stronza^?

b: Mi dispiace umana. 

b: Dovrò usare il mio ATTACCO SPECIALE. 

```
bb({body:"special_a"});
music('battle', {volume:0.5});
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act2h_attack) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act2h_attack) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act2h_attack) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`

# act2h_attack

```
bb({body:"special_b_1"});
hong({body:"forward", mouth:"forward"});
sfx("charging");
```

h: Ch'è sta ^merda^?

h: Hai intenzione di blaterare un altro po'--

```
bb({body:"special_c"});
sfx("hadouken");
```

(...901)

(#act2i)

# act2i

```
publish("hide_tabs");
publish("show_special_attack");
Game.FORCE_CANT_SKIP = true;
music(null);
stopAllSounds();
```

(...5000)

```
publish("show_tabs");
hong({ body:"final", mouth:"final" });
bb({ body:"normal", mouth:"normal", eyes:"sad" });
attack("100p", _.SPECIAL_ATTACK);
Game.FORCE_CANT_SKIP = false;
setTimeout(function(){
	publish("remove_special_attack");
},30);
```

(...2500)

h: CHE ^CAZZO^ ERA

b: Mi spiace. Dovevo mostrarti le conseguenze. 

{{if _.SPECIAL_ATTACK=="harm"}}
h: POTEVO *VEDERE* IL MIO STESSO CADAVERE. POTEVO *SENTIRE* LA SENZAZIONE DI ESSERE MORTA. 
{{/if}}

{{if _.SPECIAL_ATTACK=="alone"}}
h: POTEVO *VEDERE* LO SGUARDO DISGUSTATO DI TUTTI. POTEVO *SENTIRE* TUTTE LE COSE CHE DICEVANO. 
{{/if}}

{{if _.SPECIAL_ATTACK=="bad"}}
h: POTEVO *SENTIRE* LE MIE COSTOLE FRANTUMARSI. POTEVO *ASSAPORARE* IL SANGUE NELL'ARIA. 
{{/if}}

b: Mi spiace, umana.

n: *FINISCILA* 

[{COMBATTI: Dalle un pugno.}](#act2j_fight) `Game.OVERRIDE_CHOICE_LINE=true`

[{SCAPPA: Andiamocene da qua.}](#act2j_flight) `Game.OVERRIDE_CHOICE_LINE=true`

# act2j_fight

`bb({ eyes:"angry" });`

b: Quella psicopatica si stava approfittando di te.

b: Stava cercando di corromperti, di rovinarti tanto quanto lei! 

`bb({ body:"yell_angry_1" });`

b: Picchiala! Falle vedere le stelle! 

`bb({ body:"final_1" });`

b: PICCHIALA PICCHIALA PICCHIALA PICCHIALA PICCHIALA PICCHIALA PICCHIAL--

`_.a2_ending = "fight";`

(#act2k)

# act2j_flight

b: I *knew* all these partygoers were deeply messed up. They all dull their pain with horrible things! *Sapevo* che tutti quei festaioli erano messi male. Soffocano il loro dolore con cose orribili! 

`bb({ body:"yell_1" });`

b: E cercano di fregarti per farti fare lo stesso! Ti corrompono! Dobbiamo andarcene! 

`bb({ body:"final_1" });`

b: USCIAMO DA QUA USCIAMO DA QUA USCIAMO DA QUA USCIAMO DA QUA USCIAMO DA Q--

`_.a2_ending = "flight";`

(#act2k)

# act2k

```
Game.clearText();
publish("act2-in-4");
publish("hp_hide");
music('party1', {volume:0.6, fade:1.5});
```

(...2001)

```
publish("act2",["party_hong",26]);
sfx("slide");
```

(...1001)

```
publish("act2",["party_hunter",14]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Stai bene, ragazza?


`publish("act2",["party_hunter",13]);`

{{if _.a2_ending=="fight"}}
(#act2k_fight)
{{/if}}

{{if _.a2_ending=="flight"}}
(#act2k_flight)
{{/if}}

# act2k_fight

```
Game.clearText();
publish("act2",["party_hunter",21]);
publish("act2",["party_hong",33]);
music(null);
sfx("hit");
```

(...1000)

```
sfx("record_scratch");
publish("act2",["party_hunter",22]);
publish("act2",["party_hong",34]);
publish("act2",["dee",6]);
publish("act2",["dum",6]);
```

r: T-tu...

```
publish("act2",["party_hunter",23]);
publish("act2",["party_hong",35]);
publish("act2",["dee",5]);
publish("act2",["dum",5]);
music('party1', {volume:0.6, fade:6});
```

r: sei *perversa*

r: Mi piace. Torna alla mia festa il weekend prossimo, dolcezza. 

```
publish("act2",["party_hunter",19]);
publish("act2",["party_hong",36]);
```

h2: ok ciao, bye, adios, au revoir

r: L'animale potrebbe aver vinto oggi, ma torna e ti farò qualcosa di ancora più forte!

h2: sayōnara, auf wiedersehen, zài jiàn, shalom

r: Io e te, tesoro, mostreremo a quella bestia chi è il capo! 

(#act2k_end)

# act2k_flight

`publish("act2",["party_hong",36]);`

h2: ok scusa devo correre 

`publish("act2",["party_hunter",16]);`

r: ^dannazzione^. L'animale ha vinto oggi, uh? 

`publish("act2",["party_hunter",15]);`

h2: no no, solo, uh, devo correre una maratona. in fretta. 

`publish("act2",["party_hunter",19]);`

r: Torna il prossimo weekend, bellezza. ti farò qualcosa di ancora più forte. 

h2: ok grazie ora corro corro corro corro 

r: Io e te, tesoro, mostreremo a quella bestia chi è il capo! 

(#act2k_end)

# act2k_end

```
Game.clearText();
publish("act2-out-5");
publish("act2-outro", ["end1"]);
music("hum", {fade:2, volume:0.6});
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2500)

```
publish("act2", ["act2_end",2]);
sfx("whoosh");
```

(...1000)

b: Umana! Tutto okay?!

```
publish("act2", ["act2_end","next"]);
```

b: Accidenti, è stato *rischioso*. Potremmo a-- 

```
Game.clearText();
publish("act2", ["act2_end","next"]);
music(null);
sfx("squeak");
```

(...1500)

```
publish("act2", ["act2_end","next"]);
sfx("hit");
```

(...1000)

h: Tornerò il prossimo weekend. 

h: La prossima volta che combattiamo, non solo ti *sconfiggerò*...

h: Ti *ucciderò*, ^cazzo^.

```
Game.clearText();
publish("act2", ["act2_end","next"]);
sfx("concrete_step1");
````

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step2", {volume:0.8});
```

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step3", {volume:0.5});
```

(...901)

`sfx("concrete_step4", {volume:0.25});`

(...3000)

`_.INTERMISSION_STAGE = 2;`

(#intermission)
