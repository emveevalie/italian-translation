# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[PLAY!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Quindi, prima di iniziare, come *ti* piacerebbe leggere? 
`publish("show_options_bottom")`

# intro-start-2

n3: Ora, iniziamo la nostra storia...
```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: QUESTA É UN UMANA

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: E QUESTA É L'ANSIA DELL'UMANA

n: *TU* SEI L'ANSIA
(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: No, assolutamente no. Non ascolto. Controllerò il mio cellulare. 

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: IL TUO LAVORO É PROTEGGERE L'UMANA DAI *PERICOLI*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Accidenti! Stai scrollando via la tua vita su Twitter! Di nuovo!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Mi chiedo proprio perché non mi siedo ad ascoltare i miei pensieri piú spesso.

`hong({eyes:"neutral"});`

n: VELOCE, AVVERTILA DEL *PERICOLO!*
```
bb({eyes:"look"});
```

[Oh no, guarda che terribile notizia!](#act1d_news)

[Oh no, quel tweet non sarà mica su di *noi*?](#act1d_subtweet)

[Hey, la GIF di un gatto che beve del latte!](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h:  Heh sì, è carino, Io---

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b:  I GATTI NON RIESCONO A DIGERIRE IL LATTE E SIAMO DELLE TERRIBILI PERSONE A GUARDARE ABUSO SUGLI ANIMALI

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```


