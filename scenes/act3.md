# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: Alla salute!

```
publish("act3",["roofhunter",1]);
publish("act3",["roofhong",1]);
sfx("drinking");
```

(...4001)

```
publish("act3-alpha", ["dizzyhunter",1]);
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",3]);
```

h2: *Ah*, proprio quel che ci voleva.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: Sai, ragazza...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: Nello specifico, proprio ciò che volevano la mia amigdala destra e sinistra. 

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: Mi ricordi di me stessa da giovane. Quando ero tormentata dall'animale nella mia testa. 

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: Sono grata di poter aiutarti a uccidere la tua bestia come io ho ucciso la mia. 

```
publish("act3",["roofhunter",2]);
```

r: Hey, domanda veloce: obbligo o ver--

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: OBBLIGO!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: Haha! Grande.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: Ok. La vedi quella piscina blu laggiù? 

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: Sì? Quella sei piani sotto?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: Saltaci.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: Aspe, cosa?

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: L'animale ha iniziato a frignare, non è vero?

```
publish("act3",["roofhunter",23]);
```

r: *Oh nooooo è pericoloso, non farloooooo.*

```
publish("act3",["roofhunter",22]);
```

r: Questo è esattamente il motivo per cui abbiamo bisogno di sfidare la morte! Fare festa! Carpe diem! Sniffare coca dal ^culo^ di una prostituta, #YOLO!

```
publish("act3",["roofhunter",10]);
```

r: Mostra all'animale che non ce ne frega un ^cazzo^ delle sue lagne! Salta.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: Uh, però a volte, um... la paura ha un senso...

```
publish("act3",["roofhunter",5]);
publish("act3",["roofhong",12]);
music(null, {fade:2});
```

r: ...

```
publish("act3-alpha", ["dizzyhunter",0]);
publish("act3",["roofhunter",6]);
publish("act3",["dd",1]);
```

r: Perdonami, non ti farai mica ingannare da quella propaganda da due soldi che dice che stare male è un *bene?*

```
publish("act3",["roofhunter",17]);
```

r: Gli ^stronzi^ che comandano il mondo fanno venire a *noialtri* ansia e depressione, 

```
publish("act3",["roofhunter",18]);
```

r: poi fanno dei TED Talks per dirci di "accettare" l'^inculata^ e "abbracciare" quel demone sadico nelle nostre teste!

```
publish("act3",["roofhunter",6]);
```

r: Senti, io so che *tu* sai che l'animale *ferisce* persone come noi. *Tortura* persone come noi. 

```
publish("act3",["roofhunter",19]);
```

r: Non è nostro amico. È una bestia feroce, che deve o essere *tranquillizzata*,

```
publish("act3",["roofhunter",20]);
```

r: O ricevere *un proiettile tra gli occhi*.

```
publish("act3",["roofhunter",27]);
```

r: Diversamente, lo lascerai vincere.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: No. Ti sbagli.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
	music('battle_dark_loop');
});
```

h2: Non lo lascerò vincere.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: ^Cazzo^ sì! Credo in te, tesoro! Uccidilo <3

(#act3a)



# act3a

```
Game.clearText();
publish("act3-out");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
_.act3_bb_body = 1;
```

(...1500)

```
publish("hp_show");
```

b: no no no no no no

n: QUESTO CAPITOLO HA DUE POSSIBILI FINALI. UNO È *MOLTO, MOLTO BRUTTO*

b: NO NO NO NO NO NO NO NO NO NO NO NO NO NO

n: SCEGLI ATTENTAMENTE. PROTEGGI LA TUA UMANA.

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: AAAAAAAAAAAAAAAAAA

`bb({ mouth:"normal" });`

n: BUONA FORTUNA

```
Game.clearText();
bb({ eyes:"start" });
```

[Umana, potresti veramente MORIRE qui!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[Questo è stupido e autodistruttivo!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[Questi pazzi non sono veramente tuoi amici!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: H--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: T--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: T--

(#act3a_after)

# act3a_after

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: You know, I might've believed you... if you hadn't tried that a zillion times before. Sai, potrei averti creduto...se non avessi già provato questa tecnica un miliardo di volte. 

h: Tu sei il lupo che gridò al lupo. 

```
bb({ eyes:"sad" });
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act3_fork) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act3_fork) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act3_fork) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`


# act3_fork

```
Game.clearText();
bb({body:"special_attack"});
sfx("charging");
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
Game.FORCE_CANT_SKIP = false;
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Hai già provato anche quello.

b: umana, perfavore...

`hong({ eyes:"look_right" });`

h: Oh *mi spiace* se Big Pharma non approva i miei metodi di cura.

h: Guarda ^stronzo^, abbiamo *tutti* un modo di farti stare zitto.

`hong({ body:"look_up", eyes:"look_up" });`

h: Alcune persone si buttano sul lavoro.

`hong({ body:"look_down", eyes:"look_down" });`

h: Alcune persone si buttano su sesso, droghe e ricaricare il feed di Facebook. 

`hong({ body:"normal", eyes:"look_right" });`

h: Alcune persone si buttano su altre persone. 

`hong({ eyes:"angry" });`

h: Io mi butterò in quella piscina. 

[Sei ubriaca EDÈ PIANI SOTTO DI NOI](#act3_bad_1_harm)

[Dannazione, mi ringrazi così?!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[Okay, lo ammetto. Ho sbagliato.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: Anche se atterri in acqua, la tensione della superficie ti spaccherà le costole e ti lascerà un trauma cranico, *nel migliore dei casi!*

h: Eh.

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Ho visto un tipo russo farlo su Youtube una volta.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: I- Perdonami, *ringraziamento?*

`bb({ eyes:"angry" });`

b: Questo è esattamente perché *esisto!* Perché non ci si può fidare degli umani per proteggersi da soli!

b: Ho cercato di proteggerti le chiappe tutta la mia vita e ora tu vuo--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_good_1

`hong({ body:"laugh_1" })``

h: heh.

`hong({ body:"laugh_2" })``

h: hahahaha

`hong({ body:"laugh_3" })``

h: HAHAHAHAHAHA

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: Oh WOW questo si che è lo sminuimento del ^fottuto^ secolo!

`hong({ body:"yell_2" });`

h: Sì, tu mucchio di ^merda^ marcia! Hai fatto una ^cazzata^! 

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Qualche altra considerazione, Capitan Ovvio?

[Prendersela con me non è la risposta!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Ma questa volta  ho *veramente* ragione!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Ti ho ferito.](#act3_good_2a)


# act3_good_1_fail_revenge

b: Dovresti avere una relazione più sana con le tue emozioni piuttosto che affogarle con--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)



# act3_good_1_fail_harm

b: Perciò, perfavore, metti giù la bottiglia e--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)




# act3_bad_2

`bb({ eyes:"sad" });`

b: perfavore... non...

h: La tua barra dell'energia mi sembra tremendamente bassa, lupo, o no? 

h: Se fossi in te, sceglierei attentamente le mie prossime parole. 

`bb({ eyes:"normal" });`

[Va bene. Ho chiuso col proteggerti](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[Ho sempre avuto ragione.](#act3_bad_2_right)

[Mi dispiace.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: Bene, salta pure. Vedi quanto me ne importa. 

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: Okay bene. Alla salute. 

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: NO ASPETTA QUELLA ERA PSICOLOGIA INVERSA AVRESTI DOVUTO FARE *L'OPPOSTO* DI QUELLO CHE H--

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: *Ti* stai mettendo in pericolo. I tuoi "amici" ti *stanno usando*. E *tu* stai usando i tuoi "amici".

`bb({ eyes:"sad" });`

b: Perciò umana perfavore...Perché non mi credi?!

h: Because you never believed in *me*. Perché tu non hai mai creduto in *me*.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: Gli altri lupi da guardia hanno umani che cercando effettivamente di allenarli con pazienza, di *imparare* a lavorare insieme

b: piuttosto che semplicemente odiarli perché cercano di proteggerli! Perchè non puoi sempli--
`bb({ eyes:"normal" });`

h: Risposta sbagliata. 

(#act3_bad_3)



# act3_bad_3

```
music(null);
hong({body:"drink"});
bb({body:"attacked"});
publish("bb_STOP_VIBRATING");
attackBB("100p");
```

(...2000)

```
hong({ body:"normal", mouth:"normal", eyes:"normal" });
bb({ body:"dead" });
```

(...999)

h: *L'unica cosa di cui aver paura è la paura"*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"Non preoccuparti, sii felice!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: Tutti i saggi del nostro tempo son d'accordo: le emozioni negative son *cattive*!

`hong({ eyes:"less_angry" });`

h: Ma dai! Perché pensi siano chiamate *negative*?

b: umana... perfavore...

`hong({ eyes:"normal" });`

h: Un po' di tempo fa ho detto: "Vorrei essere libera da tutto questo dolore".

h: Il mio desiderio si è esaudito. Non sento più dolore, paura, ansia...

h: Non sento più niente.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: Ero così ossessionato dal far sì che nulla ti ferisse che non mi sono accorto di essere *io* ciò che ti feriva. 

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: MA.DAI. 

`hong({ body:"yell_1" });`

h: ^CAZZO^. Ti ci è voluto tutto questo tempo per capirlo?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: Potresti averci risparmiato così tanti problemi, tu soffice ^coglione^. Perché non te ne sei accorto prima?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...ti *dispiace*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: Ti dispiace per *cosa*?

(#act3_good_2q)


# act3_good_2q

`bb({mouth:"sorry", eyes:"sorry"});`

{{if _.apologized_for_hurt}}
(#act3_good_2q_already_apologized)
{{/if}}

{{if !_.apologized_for_hurt}}
(#act3_good_2q_not_already_apologized)
{{/if}}


# act3_good_2q_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"less_angry" });`

[Mi spiace se non sono stato un buon protettore.](#act3_good_3_protector)

[Mi spiace non averti rispettato.](#act3_good_3_respect)

[Mi spiace.](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[Mi spiace di avere una terribile umana](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[Mi spiace non averti rispettato.](#act3_good_3_respect)

[Mi spiace averti ferito.](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: È mio dovere avvertirti riguardo al *vero* pericolo, ma ho sempre abbaiato a macchine e postini. 

`bb({eyes:"sorry_up"});`

b: Abbiato alle ombre. Abbaiato così tanto. 

`bb({eyes:"sorry"});`

b: È perfettamente sensato che tu voglia zittirmi. 

`bb({eyes:"sorry_down"});`

b: Mi dispiace.

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: Avrei dovuto essere il *tuo* fedele cane da guardia, ma mi sono comportato come se tu avessi dovuto *ubbidirmi*

`bb({eyes:"sorry_up"});`

b: C'è una sottile differenza tra protettore e guardia carceraria, e io sono andato ben oltre il limite. 

`bb({eyes:"sorry_down"});`

b: Mi dispiace.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: Ero così ossessionato dal far sì che nulla ti ferisse che non mi sono accorto di essere *io* ciò che ti feriva. 
`bb({eyes:"sorry_up"});`

b: Sono stato un cane cattivo.

`bb({eyes:"sorry_down"});`

b: Mi dispiace.

(#act3_good_4)


# act3_good_4

```
music(null,{fade:3});
hong({ eyes:"less_angry", MOUTH_LOCK:true },0);
```

h: ...

```
hong({ body:"stop", mouth:"stop", eyes:"blank" });
```

h: Beh, okay, tanto era un'idea stupida. 

h: L'ho fatto solo per farti incasinare, e ce l'ho fatta. 

h: Chiamiamo questo round un pareggio, ok?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Okay.

h: Okay.

n: *PAREGGIO*

`_.a3_ending = "walkaway";`

(#act3_end)









# act3_end

```
Game.clearText();
publish("act3-in");
publish("hp_hide");
Game.FORCE_CANT_SKIP = true;
```

{{if _.a3_ending=="walkaway"}}
(#act3_walkaway)
{{/if}}

{{if _.a3_ending=="jump"}}
(#act3_jump)
{{/if}}






# act3_walkaway

```
publish("start-walkaway-anim");
Game.WORDS_HEIGHT_BOTTOM = 205;
```

(...3501)

```
sfx("bottle_toss");
publish('hong-next');
publish("act3",["roofhunter",7]);
```

(...667)

```
publish("act3",["dd",4]);
publish("act3",["roofhunter",26]);
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("concrete_step2");
```

(...667)

```
publish('hong-next');
publish("act3",["roofhunter",27]);
```

`Game.FORCE_CANT_SKIP = false;`

r: Oh, *ma dai*. Dopo tutto ciò che ti ha fatto quell'animale, vuoi semplicemente *arrenderti*?

r: Qual'è il problema? Hai *paura*?

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Sì.

h2: Ho paura.

`publish('hong-next')`

h2: E va bene!

`publish('hong-next')`

h2: Avere paura va bene.

`publish('hong-next')`

(...500)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1167)

```
publish('hong-next');
```

(...833)

```
publish('hong-next');
sfx("rustle2");
```

(...1333)

```
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",31]);
sfx("concrete_step4");
```

(...667)

```
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("door");
```

(...1333)

```
publish('hong-next');
sfx("concrete_step2");
```

(...501)

```
publish('hong-next');
Game.FORCE_CANT_SKIP = false;
sfx("lock_door");
publish("act3",["roofhunter",32]);
```

(...2001)

```
publish("act3",["roofhunter",33]);
```

r: Ma ha chiuso la porta a chiave?

```
Game.clearAll();
_.INJURED = false;
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2000)

(#act4)




# act3_jump

```
publish("start-jump-anim");
Game.FORCE_TEXT_Y = 300;
```

(...2001)

```
publish('hong-next');
sfx("bottle_toss");
```

(...833)

```
sfx("concrete_step1");
sfx("claps");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",28]);
```
(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step2");
publish('hong-next');
publish("act3",["roofhunter",28]);
```

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",34]);
```

(...1167)

```
sfx("rustle2");
publish('hong-next');
```

(...1001)

`publish('hong-next')`

b: no...

(...501)

`Game.clearText();`

`publish('hong-next')`

(...1333)

```
sfx("quack");
publish('hong-next');
```

(...1333)

`publish('hong-next')`

b: no no no

(...501)

`Game.clearText();`

`publish('hong-next')`

(...2001)

```
sfx("rustle2");
publish('hong-next')
```

(...501)

```
sfx("concrete_step1");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",30]);
```

(...167)

```
sfx("concrete_step2");
publish('hong-next');
```

(...167)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",2]);
publish("act3",["roofhunter",15]);
```

(...167)

```
sfx("bottle_slip");
publish('hong-next');
publish("act3",["dd",3]);
publish("act3",["roofhunter",16]);
```

(...833)

```
sfx("rustle");
publish('hong-next');
```

(...167)

`publish('hong-next')`

(...167)

```
publish('hong-next');
Game.FORCE_TEXT_Y = 325;
Game.OVERRIDE_FONT_SIZE = 50;
```

b: NO!

(...400)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-injury-show");
publish("hide_tabs");
```

(...2000)

```
sfx("hospital1");
publish("act4-injury", [1]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital2");
publish("act4-injury", [2]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital3");
publish("act4-injury", [3]);
```

(...8000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...5500)

`_.INJURED = true;`

(#act4)
