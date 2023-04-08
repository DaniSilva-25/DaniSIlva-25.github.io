# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: (Jogo foi auto-salvo)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *vish*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Então, qual que foi a moral desta maldita história?

`hong({body:"one_up", eyes:"annoyed"})`

h: O que é que sequer *aprendemos* com isso? Eu *estava* a ser imbecil, aqueles "colegas" *estavam* a usar-me, e quase *morremos*.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[É, sem mencionar a conta do hospital.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[É, sem mencionar o dano no fígado.](#act4a_liver)
{{/if}}

[Pois, aquele *foi* o cenário de pior caso.](#act4a_worst)

[Pois, eu disse.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: Certo. Eu não acho que o meu seguro de saúde cobre "idiotisse".

`hong({eyes:"annoyed", mouth:"normal"});`

b: E mesmo assim... sobrevivemos!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Não te enganes, nós definitivamente perdemos alguns anos da nossa expectativa de vida...

`bb({eyes:"surprise"});`

b: Mas, pelo menos, ainda *temos* alguma expectativa de vida! Sobrevivemos!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: E mesmo assim...

h: Hm?

`bb({eyes:"surprise"});`

b: Sobrevivemos!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: Mas... Disseste alguma coisa certa, também.

`hong({eyes:"surprise"});`

h: Hm?

`bb({eyes:"normal"});`

b: Eu *era* o lobinho que gritou lobo. Daí, quando perigo *de verdade* apareceu, tu – justificadamente – não acreditaste em mim.

`bb({eyes:"surprise_r"});`

b: E mesmo assim, sobrevivemos!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: Apesar de tudo, ainda estamos aqui.

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h: Estás calmo para alguém que acabou de ter que partilhar uma experiência de quase morte.
{{/if}}

{{if !_.INJURED}}
h: Estás calmo para alguém que acabou de partilhar uma experiência de *quase*-quase morte.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: Bem, isso fez tudo parecer menos assustador em comparação. E também, fez-me pensar.

`bb({eyes:"normal", mouth:"normal"});`

b: Se eu brigar contigo é porcaria, porque não te protege...

h: Mas eu brigar contigo *também* é porcaria, porque só te faz gritar ainda mais alto...

`bb({eyes:"normal_r"})`

b: Então talvez...

`bb({eyes:"normal"})`

h: Talvez não precisamos de brigar.

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: Eu não sou o Lobo Mau. Mas, eu também não sou um lobo-da-guarda.

`bb({eyes:"sad_d"})`

b: Eu sou um cão perturbado, de um abrigo.

`bb({eyes:"sad"})`

b: Já passamos por coisas bem pesadas. Talvez algum trauma, ou abandono. É por isso que eu reajo as vezes e faço:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: AU AU AU AU AU AU 

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: Mas eu não *quero* ser um cão medroso! Eu quero proteger-te! Eu quero ser um bom cão!

`bb({eyes:"sad", mouth:"normal"});`

b: Humano... podes me ajudar a treinar este lobo?

`hong({eyes:"sad"})`

h: Eu... eu vou tentar.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: Okay. Uma relação saudável com as emoções. Relacionamentos precisam de comunicação. Então, vamos nos comunicar.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: Olha, os próximos 5 minutos vão ser bem seca, mas vamos fingir que não é para que isso dê certo.

```
hong({body:"hands_2", mouth:"normal"});
```

h: Querido lobo interior... como é que *tu* te sentes agora?

n2: TOTAL DE MEDOS UTILIZADOS:

n2: *MAGOAR* {{_.attack_harm_total}}, *DESAMADO* {{_.attack_alone_total}}, *MÁ PESSOA* {{_.attack_bad_total}}

n2: SOBRE QUAL MEDO QUERES FALAR A RESPEITO PRIMEIRO? (PODEMOS FALAR DOS OUTROS DEPOIS)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Eu tenho medo que vamos ser magoados.](#act4_harm)

[Eu tenho medo de ficarmos na solidão.](#act4_alone)

[Eu tenho medo que somos má pessoa.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: Eu quero proteger a tua necessidade de segurança física,

`bb({eyes:"sad_d"})`

b: Mas o *mundo inteiro* parece tão perigoso. Tão cheio de tragédia, e mal.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: Eu sei lá, já chega de ser *eu* escolher o que dizer depois. O que é que *tu* tens a dizer, humano?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Denovo a tua vez, humano. O que é que achas?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Mais algum pensamento, humano?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Dize bem. Então, vamos nos proteger.](#act4_harm_skills)

[Vamos nos expor para *mais* perigo.](#act4_harm_exposure)

[Eu agradeço-te.](#act4_thanks) `_.thanks_for = "segurança física";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Mas... como? Posso ter garras e presas, mas eu sou apenas uma metáfora.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Talvez poderiamos aprender auto-defesa? Participar numa comunidade que se protege? Melhorar a nossa saúde e os nossos limites pessoais?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Talvez, mas...

[Por onde devemos começar?](#act4_harm_skills_start)

[Mas e se não funcionar?](#act4_harm_skills_work)

[E se nós ficarmos com *demasiada* segurança?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: Há tanto a fazer, tanto que devemos arrumar sobre nós. Por onde é que sequer começamos?

`hong({ body:"shrug", eyes:"surprise" })`

h: Nós estamos a começar agora mesmo.

`bb({ eyes:"normal", mouth:"narrow" })`

b: Eh?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Estamos a praticar uma boa comunicação agora mesmo. O que irá nos ajudar a detetar perigo com mais eficácia, com menos falsos alarmes,

`hong({ eyes:"surprise" });`

h: E *isso* vai nos ajudar a proteger de nos magoarmos!

`hong({ eyes:"normal", mouth:"normal" });`

h: Portanto: isso *já é* treino de auto-defesa.

`bb({ eyes:"normal_r" })`

b: Huh. Eu estava a esperar mais disso:

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: Mas é verdade, não há maneira de nos protegermos 100%...

`hong({ body:"one_up" });`

h: Entretanto, até uma melhoria de 1% já vale alguma coisa. Não é?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: Ainda estás a ver o copo, não como 99% vazio, mas 1% cheio?

`bb({ eyes:"normal" });`

h: O que já vale alguma coisa, se estiver perdido no meio de um deserto.

`bb({ eyes:"closed" });`

b: Bem. Enche o bico, então.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: Eu digo, o motivo de tu teres ignorado os meus alertas era justamente *porque* eu focava demasiado na tua segurânça!

`bb({ body:"normal", eyes:"normal" })`

h: Né, estás certo. Nos gostariamos de praticar segurança em moderação. Tudo em moderação.

`bb({ eyes:"suspect" })`

b: Desculpa, *TUDO* em moderação?

`hong({ eyes:"annoyed" })`

h: *Uma moderada quantidade de coisas* em moderação.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Obrigado por fazeres as tuas constatações tão recursivamente auto-consistentes.

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *O QUE*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Eu quero dizer, imagina um cão com medo de trovoada.

`hong({ body:"hands_1" });`

h: Um truque que os treinadores fazem é tocar uma gravação de trovoada em volume baixo, e dá-lo um biscoito por ficarem calmos.

`hong({ body:"hands_2" });`

h: Dentro de vários dias, o treinador aumenta o volume de pouco e pouco, até que o cão supere o medo de trovoada.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Isso chama-se terapia por exposição!

`hong({ body:"point", eyes:"normal" });`

h: Já que és um cão, isso deve funcionar contigo também, não é? Todos os mamíferos possuem o mesmo instinto de lutar-ou-fugir.

`hong({ body:"normal" });`

[Mas e se nós nos dessensibilizarmo-nos?](#act4_harm_exposure_overboard)

[Mas e se formos expostos a perigo *real*?](#act4_harm_exposure_hurt)

[Eu sou um lobo, não um cão.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: E eu vou mostrar paciência e bondade contigo, até que te tornes um cãozinho fofo e domesticado.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: D'aw.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: Nós *acabamos* de ver o que acontece quando desligas os teus medos – acabas em situações *realmente* perigosas.

`bb({ eyes:"angry_r", body:"one_up" })`

b: Além disso, se desensibilizarmos *demais* não viraríamos psicopatas?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: Em breve estaríamos a dar-nos biscoitos enquanto assistimos pornografia com homicídios!

`hong({ eyes:"annoyed" })`

h: Eu... acho que há uma linha a separar isso aí e a trovoada.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: Mas exatamente *onde*, humano? *Onde?!*

`hong({ eyes:"surprise", body:"one_up" })`

h: Eu não sei. Mas, *tu* podes me ajudar!

`hong({ eyes:"normal", body:"normal" })`

h: A trabalhar e negociar contigo, nós vamos pintar essa linha.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: Tá bem. Mas eu não tenho polegares, então quem vai ter que pintar és tu.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: Por exemplo: Nós pulamos de um maldito *telhado*!
{{/if}}

{{if !_.INJURED}}
b: Por exemplo: Nós quase pulamos de um maldito *telhado*!
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Né, estás certo. Dá *sim* para ir longe demais.

`hong({ eyes:"normal" });`

h: Mas isso também é o porquê de, se fizermos terapia por exposição, nós começamos com pouco, e vamos subindo com pequenos passos.

h: Logo antes de antingirmos perigo *de verdade*, paramos.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: É, eu digo que o limite está entre ouvir trovoada bem alta e ficar no meio de uma tempestade com um chapéu pontiagudo de metal.

(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: Espera, sem argumentos, nem a favor ou contra o que sinto? Apenas... "eu agradeço-te"?

`hong({ eyes:"surprise", body:"shrug" })`

h: Sim! Eu agradeço-te por mostrares preocupação pela minha {{_.thanks_for}}.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Estás bem?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Nunca *me agradecestes* antes.

`hong({ mouth:"smile" });`

h: Aw, seu lobão peludinho e medroso.

(#act4_something_else)

# act4_thanks_2

h: Mesmo que reajas em excesso, eu estou feliz que cuidas da minha {{_.thanks_for}}.

`bb({ eyes:"annoyed" })`

b: Espera... não estás apenas a repetir agradecimentos para evitar falar sobre os teus medos, não é?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Bem, isso é complicado, e nem sempre eu tenho respostas prontas.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: Não é como se a vida te desse uma lista de 3 respostas de diálogo prontas.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Mas por enquanto, posso no mínimo agradecer.

b: Bem, eu também te agradeço, por ouvires o que digo pacientemente.

`bb({ eyes:"closed" });`

b: Seu ser mamífero sem pelo.

(#act4_something_else)

# act4_thanks_3

h: Mesmo que os teus latidos assustem-me, tu simplemente estás a tentar proteger a minha {{_.thanks_for}}.

`bb({ eyes:"smile_r" });`

b: Tá, se continuares a ser assim comigo, a internet vai inventar umas idéias *estranhas* sobre nós.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: O que foi, sou apenas uma pessoa jovem e vulnerável enquanto tu és um grande lobo assustador. O que é o pior que eles poderiam invent--

`hong({ eyes:"normal", body:"point" });`

h: Na real, não responda isso.

(#act4_something_else)




# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: Eu quero ter certeza que tu preenchas aquele profundo sentimento humano de pertencer...

`bb({ eyes:"sad_u" });`

b: Mas me preocupo que, se alguém nos conhecesse - *realmente* - apenas iamos espantar eles.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: Eu sei lá, chega de *eu* escolher o que dizer depois. O que *tu* tens a dizer, humano?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Denovo a tua vez, humano. O que é que achas?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Mais algum pensamento, humano?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Eu concordo: vamos ajeitar a nossa vida social.](#act4_alone_skills)

[Acho que outros gostam de nos, queres saber?](#act4_alone_experiment)

[Eu agradeço-te.](#act4_thanks) `_.thanks_for = "pertencer social";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Poderíamos praticar abilidades como perguntar sobre coisas, ouvir e empatizar, ser alguém aberto e vulnéravel, etc?

`hong({ eyes:"normal_l" });`

h: Ou arranjar hábitos sociais melhores, como marcar um tempo com amigos ou ir a encontros de turma regulares?

`hong({ body:"one_up" });`

h: Também poderia aprender a ser mais confortável com rejeição.

`hong({ eyes:"normal" });`

h: Ou aprender quando é que as pessoas *não estão* nos a rejeitar-nos, sabes? Quando estão apenas cansadas, ou possuem síndrome de cara-de-^cu^.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: Isso são algumas opções. Mas, sobre "aprender abilidades sociais"...

[Isso não é meio *manipulador?*](#act4_alone_skills_manipulative)

[Isso não vai facilitar que sejamos *manipulados?*](#act4_alone_skills_manipulated)

[E se ainda der errado?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: Assassinos em série não são ótimos em ler emoções e fingir "empatia"?

`bb({ eyes:"annoyed" });`

b: Nunca ouviste falar sobre um tal de Charles Manson, líder cultista e stripper, sendo bom em fazer amigos e influenciar pessoas?

`hong({ eyes:"annoyed", body:"chin" });`

h: Então, estás certo.

h: "Abilidades sociais" não significam nada se não nos importamos *genuinamente* com as outras pessoas.

`hong({ body:"normal" });`

h: Basicamente, só não sejas um m^erd^as.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: Isso aí é pra colocar num poster motivacional.

`hong({ body:"shrug", mouth:"narrow" });`

h: “Não Sejas Um M^erd^as™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Vamo-nos tornar num tapete de boas vindas, que diz "Por favor" e "Obrigado" enquanto os outros limpam os seus pés sobre nós!

`bb({ mouth:"scream", eyes:"scream" })`

b: Vamos babar tanto ovo, até ficarmos como batom branco!

```
bb({ mouth:"normal", eyes:"normal" });
hong({ body:"chin" });
```

h: Então, estás certo. "Abilidades sociais" não podem ser apenas sobre os outros, também tem a ver com aplicar *limites*.

`hong( body:"one_up" });`

h: Não dá para convidar alguém para nossa casa se não tivermos paredes para delimitá-la.

```
hong({ eyes:"angry", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Aliás... aquela imagem do batom... *que nojo??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: Podemos falhar. Na verdade, *vamos* falhar.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: E isso não tem problema! Falhar é como todos aprendem algo novo no começo!

h: Herrar é umano.

`hong({ body:"normal", eyes:"normal" });`

h: Então vamos falhar em conjunto, tá?

`bb({ eyes:"normal_r" });`

b: Tá né, boa... no pior dos casos, podemos mudar de cidade e conseguir uma identidade nova.

`bb({ eyes:"normal" });`

h: É, eu acho que isso só custa duas bitcoins, hoje em dia.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Nós podemos exprimentar coisas para nós!

`hong({ body:"chin" });`

h: Podemos chamar um amigo para dar uma volta, reconectar com um amigo antigo, ou até conversar com a mulher do restaurante.

`hong({ body:"normal" });`

h: Acho que somos mais amigáveis do que suspeitamos.

`bb({ eyes:"annoyed" });`

[E se isso forem "vitórias" baratas e pequenas?](#act4_alone_experiment_cheap)

[E se isso aborresser essas pessoas?](#act4_alone_experiment_burden)

[Mas "conversinhas" não somos nós *de verdade*!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Se vestirmos um sorriso raso, nunca iremos ligar-nos com ninguém,

`bb({ eyes:"super_sad" });`

b: *Mas* se nós nos abrirmos, as pessoas vão ver como somos uma confusão interna!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Vira.

b: O quê.

`hong({body:"hands_1"})`

h: Quando cães querem mostrar amor e confiança, eles mostram-se vulneráveis ao expor a barriga.

`hong({body:"one_up"})`

h: Talvez não estejamos *confiantes* ainda para demonstrar vulnerabilidade, mas com treino suficiente,

`hong({body:"normal", eyes:"surprise"})`

h: Um dia talvez possamos mostrar aos outros como somos de verdade – cheio de bagunça, cheio de humanidade.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Eu vou virar se me deres um biscoito.

`bb({ eyes:"normal", mouth:"normal" });`

h: Não.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Dizer "olá" para a mulher do restaurante não é exatamente uma performance medalha-de-ouro na Olímpiada de Borboletas Sociais.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: É para *nós!*

`hong({ body:"one_up", eyes:"annoyed" });`

h: No ringue social, não somos nem peso-*pena*, somos tipo, peso-*quark*.

`hong({ body:"normal", eyes:"normal" });`

h: Se tivermos que começar com vitórias pequenas e baratas, que seja. É preciso subir o primeiro passo antes de chegar no 1000.

b: Sim! Talvez depois que dissermos "Olá", poderemos avançar e dizer...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"Como é que estás?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Estou bem!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Talvez a mulher só queira servir almoços, e não ser uma *experiência* para ver se as nossas abilidades sociais são um lixo.

`bb({ eyes:"annoyed" })`

h: Bem, se descobrirmos que estamos a ser algum problema...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Isso é bom saber, também!

`hong({ eyes:"normal" });`

h: Talvez assim possamos aprender como proativamente perguntar aos outros sobre o que é desconfortável para eles, para descobrirmos e respeitarmos os seus limites.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Sabes, toda aquela m^erd^a "interpessoal" que vemos em folhetos de conselheiros escolares.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Eu quero defender as tuas necessidades morais, que te dirigem a te tornares alguém melhor,

`bb({ eyes:"sad_d" })`

b: Mas parece que, no fundo, somos tão fundamentalmente... partidos.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: E nem me tentes dizer que não somos loucos. Nós saltamos de *um telhado*.
{{/if}}

{{if !_.INJURED}}
b: E nem me tentes dizer que não somos loucos. Quase saltamos de *um telhado*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: Eu sei lá, chega de *eu* escolher o que dizer depois. O que é que *tu* dizes, humano?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Denovo a tua vez, humano. O que é que achas?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Mais algum pensamento, humano?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Então somos partidos. Vamos arranjar isso.](#act4_bad_fix)

[Então somos partidos. Vamos aceitar isso.](#act4_bad_accept)

[Eu te agradeço.](#act4_thanks) `_.thanks_for = "integridade moral";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Podemos construir hábitos melhores devagar, alinhas a nossa vida com os nossos valores,

`hong({body:"one_up"});`

h: E, se necessário, pedir ajuda profissional – um terapeuta ou conselheiro.

`hong({body:"normal"});`

h: Existem jeitos de nos consertarmo-nos.

[Mas e se não pudermos consertar tudo?](#act4_bad_fix_cant)

[Mas e se consertarmos *demais*?](#act4_bad_fix_too_much)

[Não temos guita para ajuda profissional.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Né, acho que tens razão.

h: Não podemos consertar tudo.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Ahhh eu sabia! Sempre vamos ser partidos!

`hong({eyes:"surprise"});`

h: Mas, podemos tentar ser *menos* partidos ao menos.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Cicatrizes curam-se com o tempo, mas elas nunca desaparecem. E não têm problema nisso.

`bb({eyes:"annoyed_r"});`

b: Acho que sim. Além disso,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: Cicatrizes são *atraentes.*

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Por favor não faças isso.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: Eu sinto nojo ao admitir isso, mas... parte de mim *quer* ter essa disordem.

`bb({ eyes:"angry" })`

b: Quero dizer, sem ela, não seriamos *desinteressantes*?

`bb({ eyes:"sad_r", body:"one_up" })`

b: Sem a desordem, a nossa arte não seria sem sabor e parada?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Sem a desordem, não seríamos incapazes de ligar com os nossos colegas que também tem essa desordem?

`bb({ eyes:"sad", body:"chest" })`

b: Se ficarmos contentes com a vida, não pararíamos de tentar fazer grandes coisas?

`hong({ MOUTH_LOCK:true })`

h: ...

h: Se temos medo até de... "esgotar os nossos medos"...

h: Acho que não iremos esgotar os nossos medos.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Pois, é mesmo né! Whew! Que alívio!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Doutora, sinto ansiedade em pagar $100 a hora só para ouvir você perguntar *e como é que isso faz-te sentir?* "

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "Mm-hmm. E como é que isso faz-te sentir?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Nem, essa é preocupação é completamente razoável.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: E é realmente péssimo como planos de saúde mentais não são acessíveis para muita gente.

`hong({ eyes:"normal", mouth:"normal" });`

h: Mesmo assim, existem algumas opções baratas ou gratuitas:

`hong({ body:"chin" })`

h: Grupos de apoio, terapia online, centros de saúde de estudantes sem lucro...

`hong({ body:"hands_1" })`

h: Construção de hábitos como meditação, dormir bem, conversar regularmente com amigos, aprender coisas novas...

`hong({ body:"hands_2" })`

h: Ir para a biblioteca e alugar livros de atividades para psicoterapias comprovadas...

`hong({ body:"one_up" })`

h: Tem uma lista cheia de recursos no final deste jogo!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Bem *aquela* quarta parede não durou muito tempo.

`hong({ body:"point" });`

h: Algumas coisas são mais importantes que convenções narrativas. Como saúde mental.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Quero dizer, isso é o que terapeutas dizem, não é? Aceitar todas as tuas emoções, até as negativas?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Espere.

["Aceitar", tipo *desistir*?](#act4_bad_accept_give_up)

["Aceitar", tipo *aprovar*?](#act4_bad_accept_approve)

["Aceitar", tipo *levar literalmente*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Achas que Martin Luther King teria dito, "Não podemos sentar na parte da frente do autocarro, vamos apenas aceitar?"

`bb({ eyes:"angry_r", body:"two_up" });`

b: Porque é que o Complexo Industrial da Auto-Ajuda acha que balançar uma bandeira branca é *sabedoria profunda?*

`bb({ eyes:"annoyed", body:"normal" });`

h: Eu acho que terapeutas dizem "aceitar" coisas más com o significado de: reconhecer que elas existem e são difíceis de mudar

h: Mas não necessariamente desistir de querer realizar a mudança em sí.

`bb({ eyes:"suspect" });`

b: Então terapeutas deveriam dizer *reconhecer*, não *aceitar*.

`hong({ body:"chin", eyes:"annoyed" });`

h: É, quando penso a respeito, falar "aceitar" deixa bem confuso.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Bem, eu *reconheço* isso.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Tipo, é *bom* que somos partidos ou algo assim? Não!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Todos aqueles escritores de Hollywood que romantizam problemas mentais são fanfarrões!

`bb({ eyes:"angry", body:"two_up" });`

b: Ter um distúrbio mental é uma *porcaria!* É algo que rouba a *vida* de pessoas! Por que deveríamos "aceitar" isso?!

`bb({ body:"normal" });`

h: Acho que terapeutas dizem "aceitar" as nossas emoções com o significado de: sê paciente com elas.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Tipo como se agitar em areia movediça faz com que te afundes mais rápido, a solução é pacientemente deitar,

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Brigar contra ti, o meu temor, fez com que eu pulassse de um telhado.
{{/if}}

{{if !_.INJURED}}
h: Brigar contra ti, o meu temor, quase fez com que eu pulassse de um telhado.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Ao invés disso, a solução é fazer exatamente isso que estamos a fazer agora – não nos agitar, mas existir pacientemente um com o outro.

`bb({ eyes:"annoyed" });`

b: Então eles deveriam dizer *isso aí* ao invés de uma palavra ambígua como "aceitar".

`hong({ body:"chin", eyes:"annoyed" });`

h: É, quando penso a respeito, dizer "aceitar" deixa bem confuso.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: Eu não aceito "aceitar".

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: Mas já *sabemos* que tu não me deves entender literalmente!

`bb({ eyes:"sad_u", body:"two_up" });`

b: Todo esse *problema* é que eu quero ajudar-te, mas sou péssimo em usar palavras para fazer isso!

`bb({ eyes:"sad", body:"normal" });`

h: Eu acho que terapeutas dizem "aceita" as emoções com o significado de: "não brigues com elas ou as ignores"

`hong({ eyes:"surprise", body:"one_up" });`

h: Para te ouvir, para trabalhar *contigo*, mas não "aceitar" tudo que diz 100% como verdade absoluta.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Então eles deveriam dizer *isso aí* ao invés de uma palavra ambígua como "aceitar".

`hong({ body:"chin", eyes:"annoyed" });`

h: Eu acho que eles também são péssimos em usar palavras, também.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Enfim, há algo mais que queiras conversar?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: Então, alguma outra coisa pesanda no teu coração?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[Eu tenho medo que seremos magoados.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[Eu tenho medo de ficarmos na solidão.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[Eu tenho medo que somos má pessoa](#act4_bad)
{{/if}}

[Nem, tudo suave por agora.](#act4c_prelude)

# act4_something_else_2

h: Okay, acho que falamos sobre todos os nossos medos, até ao momento.

b: Sim, existem apenas 3 medos.

h: Sim, *exatamente* três.

b: Que conveniente.

(#act4c)

# act4c_prelude

h: Boa conversa, equipa.

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b: Isso não é algum tipo de *jogo*, sabes.

`bb({eyes:"angry_d", body:"one_up"})`

b: Construir um relacionamento saudável com as tuas emoções não é tão simples como clicar em botões numa tela.

`bb({eyes:"sad", body:"normal"})`

b: *Será* que vamo-nos dar bem?

b: *Será* que vamos conseguir trabalhar juntos, como uma equipa?

`hong({eyes:"sad", body:"one_up"})`

h: Bem,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: C-com licença...

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: Importas-te que eu almoçasse contigo?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *Aquilo* é o teu crush? Por que é que ele está sentados como um assassino em série psicopata?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Perguntar para o teu crush se podes almoçar com ele? Sabes o quanto de *desespero* isso transmite?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *Aquele* é o teu crush? Interrompemos a sua paz e tranquilidade! Somos tão maus!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: E- eu quero dizer- não, não tem problema se não posso, eu só...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Espere, não te vi naquela festa?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Sim, claro! Chega aí.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Desculpa, preciso de espaço no momento.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Sim! Estava no sofá, na primeira festa que eu fui...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Onde eu tive um ataque de pânico e dei um soco na anfitriã.
{{/if}}

{{if _.a2_ending=="flight"}}
h2:  Onde eu tive um ataque de pânico e saí a chorar.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Espera aí humano, talvez estejamos a deixá-la desconfortável.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, eu não quis acusar-te!

`publish("act4", ["hong_to_alshire",4]);`

h2: Apenas lembrei de um rosto amigável, só isso.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AHHHHH EU SABIA! ELE É ALGUM PSICOPATA PERIGOSO INDUZIDO A PÂNICO!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAHHH A PRIMEIRA IMPRESSÃO QUE FIZEMOS FOI "PRESENCIASTE O MEU TRAUMA"! ISSO SIGNIFICA QUE ELE NOS ODEIA!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAHHH FIZEMOS ALGUÉM LEMBRAR DE UM EVENTO TRAUMÁTICO. NOSSA MERA PRESENÇA MAGOA AQUELES HÁ NOSSA VOLTA.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Espera aí humano, ela parece estar desconfortável.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, sem pressão aí!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Só estou a dizer, podes comer aqui se quiseres.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: ELE ESTÁ A SER AMIGÁVEL *DEMAIS*! COMO TED BUNDY, O ASSASSINO EM SÉRIE!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: ELE ESTÁ A FINGER SER FIXE! NINGUÉM *REALMENTE* QUER QUE CHEGAMOS PERTO!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AHHH SEMPRE FAZEMOS OS OUTROS SE SENTIREM ESTRANHOS! SOMOS UMA CONFUSÃO SOBRE O PLANETA!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Espera aí humano, talvez estejamos a deixá-la desconfortável.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, eu não quis ser rude!

`publish("act4", ["hong_to_alshire", 6]);`

h2: Só preciso de um tempo para processar as minhas emoções. Por favor, não leves isso como rejeição pessoal.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: QUE PENSAMENTOS DEPREVADOS ELE ESTÁ A PROCESSAR?! QUE ESCURIDÃO PREENCHE O CORAÇÃO DE TAL PSICOPATA?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: FOMOS REJEITADOS! NUNCA SEREMOS AMADOS!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: NÓS INTERROMPEMOS O PROCESSAMENTO EMOCIONAL DELE! AGORA ELE ESTARÁ TRAUMATIZADO PARA SEMPRE E É TUDO NOSSA CULPA!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: SAI SAI SAI SAI SAI SAI SAI SAI SAI SAI

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: Huh. Aquilo foi estranho. Quero saber o que estava a acontecer na cabeça daquela pessoa.

`publish("act4", ["hong_closer", 2]);`

h: De qualquer forma, estavas a falar do que mesmo?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Uh, eu esqueci? Algo sobre equipa e trabalho?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: Eles dizem que tes que "fazer as pazes" com as tuas emoções, como se as tuas emoções fossem *criminosos de guerra!*

`publish("act4", ["bb_closer", 7]);`

b: Mas eu quero que façamos mais que as pazes! Quero que sejamos aliados!

`publish("act4", ["bb_closer", 3]);`

b: Eu quero ser um bom cão-de-guarda. Tipo como fome e sede são alarmes de as tuas necessidades físicas,

`publish("act4", ["bb_closer", 8]);`

b: Eu quero ser o alarme para as tuas necessidades *psicológicas* - as tuas necessidades por segurança, por pertencer, por fazer o que é certo.

`publish("act4", ["bb_closer", 1]);`

b: Mas... eu sou péssimo com o meu trabalho, então eu preciso que me treines.

`publish("act4", ["bb_closer", 4]);`

b: Eu não serei "sempre válido" ou "sempre irracional". Eu só... tento o meu melhor. Então, por favor...

`publish("act4", ["bb_closer", 30]);`

b: Ajuda-me a ajudar-te!

`publish("act4", ["bb_closer", 6]);`

b: Apesar de que, ensinar um cachorro velho truques novos *vai* levar um tempo. Talvez até *anos.*

`publish("act4", ["bb_closer", 3]);`

b: E as vezes vou ter relapsos, voltarei aos meus hábitos antigos.

`publish("act4", ["bb_closer", 2]);`

b: Vou ladrar para as sombras. Vou te assustar com palavras. Talvez até mostre imagens intrusivas de... coisas, para ti.

`publish("act4", ["bb_closer", 9]);`

b: Desculpa-me! Sou um cãozinho perturbado de abrigo! Cães perturbados c^aga^m na tua cama, as vezes!

`publish("act4", ["bb_closer", 4]);`

b: Mas se fores paciente comigo... se ficares e sentares comigo...

`publish("act4", ["bb_closer", 8]);`

b: Talvez consigas treinar este lobo aqui.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Bom cão.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Bom humano.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
b: AAAAA AINDA ESTAMOS A COMER SOZINHOS QUINZE CIGARROS AAAAA
{{/if}}

{{if _.parasite}}
b: AAAAA AINDA NÃO ESTÁS A SER PRODUTIVO ENQUANTO COMES SOMOS PARASITAS AAAAA
{{/if}}

{{if _.whitebread}}
b: AAAAA ESTÁS A COMER MAIS PÃO BRANCO AAAAA
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: AU AU AU AU AU AU

(#credits)