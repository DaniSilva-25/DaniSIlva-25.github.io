# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: Saúde!

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

h2: *Ah*, isto bate bem.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: Bate, jovem...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: Para ser específico: bateu bem nas minhas amígdalas cerebelosas, direita e esquerda.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: Lembras-me quando era mais jovem. Quando era alguém atormentado por um animal na minha cabeça.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: Estou feliz que posso passar isso adiante, ajudar-te a matar essa besta como eu matei a minha.

```
publish("act3",["roofhunter",2]);
```

r: Ei, pergunta: verdade or conseq--

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: CONSEQUÊNCIA!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: Haha! Boa.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: Então. Estás a ver aquela piscina azul, lá embaixo?

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: Tô? Seis andares pra baixo?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: Salta lá para dentro.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: Pera, o quê?

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: O animal começou a reclamar, não começou?

```
publish("act3",["roofhunter",23]);
```

r: *Ah nããão é perigoso, não faças issooo*

```
publish("act3",["roofhunter",22]);
```

r: Mas isso é exatamento o porquê de precisarmos destes desafios que encaram a morte! Festejar adoidamente! Carpe diem! Colocar platina no nariz, #YOLO!

```
publish("act3",["roofhunter",10]);
```

r: Mostra àquele animal que tás a c^aga^r para ele a chatear-te a cabeça! Cai dentro.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: Uh, às vezes, hum... medo tem razão...

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

r: Desculpa, acabaste de cair naquele conto "McMindfulness" onde sentimentos maus são *bons*?

```
publish("act3",["roofhunter",17]);
```

r: O Prazer é o oposto da dor. Portanto podes usar prazer para vencer a dor, c^aralh^o!

```
publish("act3",["roofhunter",18]);
```

r: Como é que aqueles pseudo-budistas do Silicon Valley não vêm essa m^erd^a?!

```
publish("act3",["roofhunter",6]);
```

r: Jovem, eu sei que *tu* sabes que esse animal apenas *magoa* gente como nós. Ele *tortura* gente como nós.

```
publish("act3",["roofhunter",19]);
```

r: Ele não é nosso amigo. É uma besta fora de controlo, o que significa que ela tem que ser ou *tranquiziliada*,

```
publish("act3",["roofhunter",20]);
```

r: Ou levar um *tiro no meio da testa*.

```
publish("act3",["roofhunter",27]);
```

r: Caso contrário, ela vai ganhar.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: Não. Estás enganado.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
	music('battle_dark_loop');
});
```

h2: Eu não vou deixar ela ganhar.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: Isso mesmo, c^aralh^o! Eu acredito em ti, amor! Dá-lhe! <3

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

b: não não não não não não 

n: ESTE CAPÍTULO POSSUI DOIS FINAIS POSSÍVEIS. UM DELES É *MUITO, MUITO MAU.*

b: NÃO NÃO NÃO NÃO NÃO NÃO NÃO NÃO NÃO NÃO 

n: ESCOLHE SABIAMENTE. PROTEJE O TEU HUMANO.

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: AAAAAAAAAAAAAAAAAA

`bb({ mouth:"normal" });`

n: BOA SORTE

```
Game.clearText();
bb({ eyes:"start" });
```

[Humano, Tu podes mesmo morrer aqui!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[Isso é estúpido e auto-destrutivo!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[Aqueles doentes não são teus amigos!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: H--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: A--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: I--

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

h: Sabes, talvez eu até acreditaria em ti... se não tivesses agido assim um zilhão de vezes antes.

h: És o pequeno lobo que gritou lobo.

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

h: Também tentaste essa porcaria de "me mostrar".

b: humano, por favor...

`hong({ eyes:"look_right" });`

h: Ah, *desculpa* se a Indústria Farmacêutica não aprova a minha auto-medicação.

h: Olha, c^abrã^o, todos *nós* temos uma maneira de te fazer fechar essa matraca.

`hong({ body:"look_up", eyes:"look_up" });`

h: Algumas pessoas atiram-se ao trabalho.

`hong({ body:"look_down", eyes:"look_down" });`

h: Algumas pessoas atiram-se ao sexo, nas drogas, em atualizar a feed de seus Facebooks.

`hong({ body:"normal", eyes:"look_right" });`

h: Algumas pessoas atiram-se a outras pessoas. 

`hong({ eyes:"angry" });`

h: Agora eu, eu vou me atirar aquela piscina.

[Estás bêbedo e são SEIS ANDARES PRA BAIXO](#act3_bad_1_harm)

[Fogo, esse é o agradecimento que eu ganho?!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[Pronto, eu admito. Eu fiz porcaria.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: Mesmo se acertares a água, dessa altura a tensão de superfície vai partir as tuas costelas e dar-te uma concussão *no mínimo!*

h: Meh.

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

h: Eu vi um Russo fazer isso no Youtube uma vez.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: D- Desculpa, o *agradecimento?*

`bb({ eyes:"angry" });`

b: Isso aqui é exatamente o porquê de *eu existir*! Devido ao facto de que não dá para confiar em humanos para se manterem seguros!

b: Estiva a tentar proteger o teu ^cu^ burro a minha vida inteira e agora tu simplesmente va--

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

h: A SÉRIO, esse é a descula mais f^odid^a do século!

`hong({ body:"yell_2" });`

h: Sim, a tua montanha de m^erd^a coberta com *sangue*! Fizeste porcaria como c^aralh^o!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Alguma outra observação, Capitão Óbvio?

[Mas vingares-te de mim não é a resposta!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Mas desta vez, eu *realmente* estou certo!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Eu magoei-te.](#act3_good_2a)


# act3_good_1_fail_revenge

b: Precisas ter uma relação mais saudável com as tuas emoções, e não afogá-las co--

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

b: Então por favor, larga essa garrafa e vamo--

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

b: por favor... não faças...

h: A tua barra de energia aí tá bem baixa, lobo.

h: Se eu fosse a ti, escolhia as minhas próximas palavras com cuidado.

`bb({ eyes:"normal" });`

[Ok. Estou farto de te proteger.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[Estive certo este tempo todo.](#act3_bad_2_right)

[Desculpa.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: Tudo bem, vai em frente e pula. Vê se eu tou-me a c^aga^r.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: Ok então. Bola de canhão.

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: NÃO, ESPERA, ISSO ERA PSICOLOGIA INVERTIDA DEVIAS FAZER O *OPOSTO* DO QUE EU DISS--

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: *Estás* a colocar-te em perigo. Os teus supostos "amigos" *estão* apenas a usar-te. E *tu* estás apenas a usar os teus supostos amigos.

`bb({ eyes:"sad" });`

b: Então por favor, humano... por que não acreditas em mim?!

h: Porque tu nunca acreditaste em *mim*.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: Outros lobos-da-guarda têm humanos que tiram tempo para treiná-los com paciência, para *aprender* a trabalhar juntos

b: Ao contrário de odiarem os seus lobos-da-guarda por tentarem protegê-los! Então por que é que não podes simplesm--

`bb({ eyes:"normal" });`

h: Resposta errada, seu idiota.

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

h: *"A única coisa que devemos temer é o próprio medo."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"Não te preocupes, sê feliz!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: Todos os sábios da nossa era concordam: emoções negativas são *más!*

`hong({ eyes:"less_angry" });`

h: Duh! Por isso que elas se chamam *negativas*!

b: humano... por favor...

`hong({ eyes:"normal" });`

h: Um tempo atrás, eu mesmo disse: “só quero ser livre de toda essa dor”

h: Eu consegui o meu desejo. Não sinto mais dor, medo, ou ansiedade...

h: Eu não sinto mais nada.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: Estive tão obsecadamente à procura de coisas que te iriam magoar, que eu não percebi que *eu* poderia estar a magoar-te.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: NÃO. DIGAS.

`hong({ body:"yell_1" });`

h: F^ODA^-SE. A sério que levaste esse tempo todo para entenderes isso?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: Poderias ter evitado tanto problema, seu grande e felpudo *zé ninguem*. Por que é que não tocaste nisso antes?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...estás a pedir *desculpas.*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: Desculpas pelo *quê*?

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

[Desculpa, por não ser um bom protetor.](#act3_good_3_protector)

[Desculpa, por não te respeitar.](#act3_good_3_respect)

[Desculpa.](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[Desculpa, por ter um humano péssimo!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[Desculpa, por não te respeitar.](#act3_good_3_respect)

[Desculpa, por te magoar](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: É o meu dever avisar-te sobre perigos *reais*, mas eu simplesmente ficava a ladrar para os carros e o carteiro.

`bb({eyes:"sorry_up"});`

b: Ladrar para as sombras. Ladrar demais.

`bb({eyes:"sorry"});`

b: Faz todo sentido quereres colocar-me numa mordaça.

`bb({eyes:"sorry_down"});`

b: Desculpa.

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: Eu devia ser o *teu* leal cão-de-guarda, mas eu agi como se tivesses de obedecer a *mim*.

`bb({eyes:"sorry_up"});`

b: Existe diferença entre um protetor e um guarda de penitenciária, e eu passei desse limite.

`bb({eyes:"sorry_down"});`

b: Desculpa.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: Estive tão obsecadamente a procura de coisas que iriam magoar-te, que eu não percebi que *eu* poderia estar a magoar-te.

`bb({eyes:"sorry_up"});`

b: Eu fui um cão mau.

`bb({eyes:"sorry_down"});`

b: Desculpa.

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

h: Bem, isso aqui foi uma má idéia de qualquer forma.

h: Só fiz isso para te mandar a baixo, e, bem, eu mandei-te bem pra baixo.

h: Vamos dizer que é um empate, tá bem?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Tá bem.

h: Tá bem.

n: *EMPATE*

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

r: Ahh *o que foi*. Depois de tudo que aquele animal fez contigo, vais *desistir?*

r: O que tens, jovem? Estás com *medo?*

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Sim.

h2: Estou com medo.

`publish('hong-next')`

h2: E não há problema nisso!

`publish('hong-next')`

h2: Não há problemas em ficar com medo.

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

r: Acabaram de trancar a porta?

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

b: não...

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

b: não não não

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

b: NÃO!

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
