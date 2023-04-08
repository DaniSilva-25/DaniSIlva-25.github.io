# act1

```
SceneSetup.act1();
```

(...300)

n: E ISTO É A ANSIEDADE DESTE HUMANO.

n: _TU_ ÉS A ANSIEDADE

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Ah, então? Aqui vamos nós outra vez.

`hong({eyes:"0_neutral"})`

n: O TEU TRABALHO É PROTEGER O TEU HUMANO DOS *PERIGOS*

`bb({eyes:"look", mouth:"small_lock"})`

n: DE FACTO, REPETIR O JOGO ESTÁ A COLOCÁ-LO EM *PERIGO* AGORA MESMO

n: RÁPIDO, AVISA-O!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Humano! Ouve, estamos em perigo! O jogador...

[...vai torturar-nos outra vez!](#act1_replay_torture)

[...não vai achar um final alternativo!](#act1_replay_alternate)

[...tem dissonância ludonarrativa!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Ele vai-te fazer enrolar numa bola e chorar!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Ele vai-nos fazer partir o teu celular ao dar-te um ataque de pânico!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Ele não vai-te deixar bater na anfitriã da festa!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Ele vai-te fazer bater na simpática anfitriã anti-herói da festa!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Bem, talvez assim não vamos pular do telhado desta v--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: ELE VAI-NOS FAZER PULAR DO TELHADO.
{{/if}}

`bb({body:"fear"});`

b: TODAS ESTAS COISAS HORRÍVEIS VÃO ACONTECER CONNOSCO, E ENTÃO VAMOS--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Tudo bem que a história em si é a mesma, mas cada capítulo possui dois finais possíveis, além de várias ramificações no diá--

`bb({body:"fear"});`

b: O jogador vai ficar desapontado, vai fechar o separador do navegador, eliminar o jogo, e então nós vamos--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Uma luso-o quê agora?

`bb({eyes:"normal"});`

b: A mensagem de história foi sobre como tu podes *ESCOLHER* construir uma relação saudável com os teus medos,

`bb({eyes:"normal_right"});`

b: Mas jogar o jogo outra vez vai resultar na mesma estória, o que implica que que as tuas *ESCOLHAS* não importam,

`bb({eyes:"narrow_eyebrow"});`

b: Irá mostrar então a contradição entre a mensagem do jogo e as suas mecânicas,

`bb({eyes:"fear"});`

b: Que logo irá desmoronar a construção deste universo narrativo,

`bb({body:"fear"});`

b: E então nós vamos--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: MOOOOORREEEEEEEEEER

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

h: Pronto, vamos voltar aos personagens.

```
Game.clearText();
```

n4: (DEIXA A _TUA_ ANSIEDADE BLÁ BLÁ BLÁ QUE MAIS SE ASSEMELHA AO QUE _TEU_ MEDO BLÁ BLÁ JÁ SABES)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Oh boa, o meu lobo voltou. Fantááástico.

`hong({eyes:"0_neutral"})`

n: O TEU TRABALHO É PROTEGER O TEU HUMANO DE *PERIGOS*

`bb({eyes:"look", mouth:"small_lock"})`

n: DE FACTO, AQUELA SANDES ESTÁ A COLOCÁ-LO EM *PERIGO* AGORA MESMO

n: RÁPIDO, AVISA-O!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Humano! Ouve, estamos em perigo! O problema é que...

`bb({body:"squeeze"})`

n4: (DEIXA A _TUA_ ANSIEDADE SAIR PARA BRINCAR! ESCOLHE AQUILO QUE MAIS SE ASSEMELHA AO QUE O _TEU_ MEDO DIZ)

(#act1_normal_choice)

# act1_normal_choice

[Estamos a almoçar sozinhos, denovo!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Não estamos a ser produtivos a comer!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Esse pão branco aí é mau para nós!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: Sabias que a solidão está associada com mortes prematuras tanto quanto fumar 15 cigarros por dia?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Hum, obrigado por citares as tuas fontes mas--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Isso significa que, se nós não convivermos com alguém *agora mesmo*, vamos--

`bb({body:"panic"})`

b: MOOOOORREEEEEEEEEER

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: USASTE O *MEDO DE SER DESAMADO*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Tira o computador para fora e trabalha nalguma coisa agora!

`hong({eyes:"0_annoyed"})`

h: Hum, eu preferiria não entornar migalhas no meu teclad--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Se não estivermos contribuindo ao corpo-da-sociedade, então nós somos um parasita-da-sociedade!

b: O corpo-da-sociedade irá ao doutor-da-sociedade para medicação exterminadora de parasitas-da-sociedade e então nós vamos--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: MOOOOORREEEEEEEEEER

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: USASTE O *MEDO DE SER MÁ PESSOA*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Tens a certeza que estes estudos foram comprov--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Trigo processado vai tirar açúcar fo sangue, e então eles vão ter de amputar todos os nossos membros, e então nós vamos--

`bb({body:"panic"})`

b: MOOOOORREEEEEEEEEER

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: USASTE O *MEDO DE SE MAGOAR*

(#act1b)

# act1b

n: É SUPER EFETIVO

`bb({mouth:"smile", eyes:"smile"});`

b: Viste, humano? Eu sou o teu lobo-da-guarda!

`bb({body:"pride_talk"});`

b: Confia no teu coração! Os teus sentimentos são sempre válidos!

`bb({body:"pride"});`

n: REDUZ A BARRA DE ENERGIA DE TEU HUMANO PARA ZERO

n: PARA PROTEGER AS SUAS NECESSIDADES FÍSICAS + SOCIAIS + MORAIS, PODERÁS USAR:

n: MEDO DE *SE MAGOAR* #harm#

n: MEDO DE *SER DESAMADO* #alone#

n: E MEDO DE *SER MÁ PESSOA* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (DICA: SELECIONA AS ESCOLHAS QUE PESSOALMENTE ATINGEM OS TEUS MAIORES, MAIS PROFUNDOS MEDOS!)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: queres saber, talvez seja hora de ir para o telemóvel.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: PROTEJE O TEU HUMANO.

n: DO MUNDO. DE OUTRAS PESSOAS. DELE MESMO.

n: BOA SORTE!

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: ROUND 1: *FIGHT!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Huh. O meu feed do facebook diz que vai haver uma festa este fim de semana.

`bb({eyes:"uncertain"});`

b: Essa pessoa não faz uma festa *todos* os fins de semana?

`bb({eyes:"uncertain_right"});`

b: Que tipo de vazio ela está a tentar preencher? Elea deve ser uma confusão por dentro!

`hong({eyes:"surprise"});`

h: E, eu recebi um convite?

`bb({eyes:"fear", mouth:"normal"});`

b: Pois então!

[Diz que sim, ou vamos morrer de solidão!](#act1c_loner)

[Diz que não, vai estar cheio de drogas!](#act1c_drugs)

[Ignora, estamos sempre a arruinar festas.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: 15 cigarros ao dia, humano! Quinze!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: E então ninguém vai ao nosso funeral, eles vão atirar as nossas cinzas ao oceano, vamos ser comidos por uma baleia,
{{/if}}

{{if !_.fifteencigs}}
b: e vamos virar M^ERD^A DE BALEIA!
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
b: Mas é, nós devemos ir para aquela festa!
{{/if}}

{{if _.parasite}}
b: Leva o computador para podermos trabalhar, e não sermos um parasita-da-sociedade.
{{/if}}

{{if _.whitebread}}
b: Espero que eles não sirvam PÃO BRANCO.
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: DEUS. Pronto, se isso te fizer calar a boca, tudo bem.

h: Vou dizer sim.

{{if _.whalepoop}}
b: M^ERD^A de baleia, humano! M^erd^a de baleia!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: ou até pior... PÃO BRANCO.
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Vamos ter uma overdose tão pesada de cocaina e pão branco que eles não vão conseguir caber o nosso cu gordo dentro do crematório!
{{/if}}

{{if !_.whitebread}}
b: Vamos ter uma overdose com tantas drogas que o funerário vai perguntar como que o nosso corpo já *tinha sido* embalsamado!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: Além disso, não podemos festejar; precisamos trabalhar ou seremos horríveis parasitas-da-socidade!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: DEUS. Pronto, se isso te fizer calar a boca, tudo bem.

h: Vou dizer não.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Tudo que fazemos em festas é reclamar num canto sobre como solidão é tão mortífera quanto fumar 15 cigarros ao dia.
{{/if}}

{{if _.parasite}}
b: Tudo que fazemos em festas é nos preocupar como deveriamos estar a ser produtivos.
{{/if}}

{{if _.whitebread}}
b: Tudo que fazemos em festas é nos preocupar como as opções de comida não saudáveis vão nos matar.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: F^oda^-se, porque será?.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Então se irmos, nós vamos fazer eles se sentirem mal, mas se rejeitarmos o convite nós também vamos fazer eles se sentirem mal!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: TUDO QUE FAZEMOS FAZ COM QUE AS PESSOAS SE SINTAM MAL, LOGO NÓS DEVEMOS NOS SENTIR MAL

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Ugh. Se isso te fizer calar a boca, tudo bem.

h: Eu vou ignorar o convite.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: De qualquer forma. Facebook tá uma m^erd^a hoje. Preciso de algo mais calmo, menos criador a ansiedade.

`hong({eyes:"neutral"});`

h: O que há no Twitter?

`bb({eyes:"look"});`

[Ah não, olha este terrível artigo de notícia!](#act1d_news)

[Ah não, será que aquele tweet era sobre *nós*?](#act1d_subtweet)

[Olha, um GIF de um gato a beber leite](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Meu Deus, é como se o mundo estivesse a arder, não é?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Parece que está tudo a acabar, como se tudo estivesse a morrer e como se nós estivéssemos perdidos com nada que possamos fazer a respeito.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: De qualquer forma, vamos retweetar esse artigo!

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

h: Tá bom, eu vou retweetar, mas por favor fica quieto!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: F^oda^-se, vou ver o Snapchat.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: É um subtweet! Um esperto subtweet sorrateiro!

`hong({eyes:"annoyed"});`

h: Provavelmente não é?

`bb({eyes:"narrow", mouth:"small"});`

b: mas e se eles estiverem a falar nas nossas costas

h: Eles n--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: NA FRENTE DAS NOSSAS COSTAS

`hong({eyes:"sad", mouth:"sad"});`

h: Eu n--

`bb({eyes:"narrow", mouth:"small"});`

b: Mas *e se for*

h: S--

`bb({eyes:"narrow_eyebrow"});`

b: *e se for*

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

h: Ok ok ok, vou ver o Snapchat.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Hehe sim é bonito, acabei de retweetar, eu ach--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: GATOS NÃO PODEM DIGERIR LEITE SOMOS PESSOAS TERRÍVEIS POR GOSTAR DE ABUSO DE ANIMAIS

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

h: o-KAY, vou ver o Snapchat.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Huh, fotos de ontem a noite. Então *é assim* que aquelas festas semanais são.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Ui, parece muita gente para a minha ansiedade.

h: Talvez eu deveria ter dito não para o convite?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Mudar de idéia? É ser estúpido?!](#act1e_yes_dontchange)

[Mudar de idéia! É muito cheio!](#act1e_yes_changetono)

{{if _.subtweet}}
[Pois é, eles estavam a subtweetar a gente mesmo.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Espera, nós retweetamos o artigo sem verificar factos.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Sabias que tu sentas-te com uma péssima postura?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Eles estavam a contar connosco para ir, e agora estamos a trair a confiança deles? Queres morrer na solidão?

{{if _.fifteencigs}}
b: QUINZE. CIGARROS.
{{/if}}

{{if _.whalepoop}}
b: M^ERD^A. DE. BALEIA.
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

h: Cala a boca cala A BOCA eu vou manter o meu sim!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Nunca ouviste falar de pisoteamento humano?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Em 2022, dezenas de milhares de pessoas foram a uma festa de Halloween em Seul num bairro pequeno, o que fez 146 pessoas serem pisadas até a morte-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: TU QUERES QUE ISSO ACONTEÇA CONNOSCO-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: DIZ QUE NÃO DIZ QUE NÃO DIZ QUE NÃO DIZ QUE NÃO DIZ QUE NÃO DIZ QUE N-


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

h: Cala a boca cala A BOCA eu vou mudar para não! DEUS!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... parece bem fixe.

h: Talvez eu não deveria ter dito não para o convite?

`bb({mouth:"normal", eyes:"normal"});`

[Mudar de idéia? É ser estúpido?!](#act1e_no_dontchange)

[Mudar de idéia! Não morras na solidão!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Pois é, eles estavam a subtweetar-nos mesmo.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Espera, nós retweetamos o artigo sem verificar factos.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Sabias que tu sentas-te com uma péssima postura?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Todos estavam a contar connosco!

b: ...em deixá-los em paz para que pudessem ter uma boa festa sem uma pessoa esquisita {{if _.whitebread}}comedora-de-pão-branco{{/if}} bizarra como tu--


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

h: Cala a boca cala A BOCA eu vou deixar como não!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Solidão crónica aumenta os níveis de cortisol juntamente ao risco de doenças cardiovasculares e derrames!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: QUINZE. CIGARROS.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Cala a boca cala A BOCA eu vou mudar para sim! Deus!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Todos os nossos tweets problemáticos vão voltar para nos crucificar!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: Nós vamos ser expostos, cancelados, arrastados pela super-autoestrada da informação por uma corda de acusações!

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

h: Por que é que tu és assim?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Nós estamos a espalhar desinformação! Destruindo a confiança popular na imprensa livre!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Somos a razão pela qual o fascismo irá se erguer sobre as ruínas da democracia!

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

h: Por que é que tu és assim?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Tu queres que a tua coluna vire um pretzel?! Para de ficar que nem um corcunda sobre a tela!

```
bb({body:"meta"});
```

b: Isso é pra ti, também.

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

h: Por que é que tu és assim?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... parece bem legal.

h: Talvez eu não deveria ter ignorado o convite?

`bb({mouth:"normal", eyes:"normal"});`

[Continua a ignorar, somos terríveis em festas ainda.](#act1e_ignore_continue)

[Na verdade, diz que sim.](#act1e_ignore_changetoyes)

[Na verdade, diz que não.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: Mas é um pouco duro continuar a ignorá-los, não é?

`bb({eyes:"normal_right"});`

b: Bem, outras pessoas sempre *ignoram-nos*, então

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: vamos dizer que é um empate.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: Tu... estás a deixar que eu me divirta?

b: Bem, digo, solidão *pode* nos matar.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: É muita gente. Multidões são perigosas.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: Tanto faz. Nova notificação no Tinder.

`bb({eyes:"uncertain"})`

b: O que, aquela app de sexo?

`hong({eyes:"annoyed"})`

h: Não é um app de sexo, é só um jeito de conhecer novas pess--

`bb({eyes:"narrow"})`

b: É uma app de sexo.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: Oh, recebi um match! Essa pessoa é bonita!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Por favor não arruines isso pra m--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: PERIGO PERIGO PERIGO PERIGO PERIGO PERIGO PERIGO 

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Estamos a ser *usados* por outros.](#act1f_used_by_others)

[Estamos a *usar* os outros.](#act1f_using_others)

[O TEU MATCH É UM ASSASSINO EM SÉRIE](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Sexo casual talvez preencha o buraco ali embaixo,

b: mas nunca vai preencher o buraco...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: aqui *dentro*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: O que estou a dizer é que, VAMOS MORRER SOZINHOS

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Achas que sexo alheio são como Pokémons para colecionar?

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

b: ♫ (música tema do pokemon)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ Esse meu jeito de ^fod^er-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ Ninguém nunca viu igual-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ A minha vida é prazer-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ Peitos, o^ra^l e ^an^al!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ PU^TA^-MON! EU VOU OS PEG-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Quero dizer que somos nojentos e manipuladores.

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
b: Eles vão te prender a um poço e forçar-te a comer pão branco para te engordar, e então vestir a tua pele como um macacão!
{{/if}}

{{if _.parasite}}
b: Eles vão te bater com um temporizador de pomodoro e dizer "TU DEVIAS TER SIDO MAIS PRODUTIVO, PARASITA"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Eles vão triturar a tua carne em confetti, transformar os teus orgãos em serpentinas, misturar o teu sangue numa bacia de ponche
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Que tal ISSO como convite de festa?!
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

h: estou a ficar doente com este jogo.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"solidão vai nos matar"... {{/if}}
{{if _.parasite}}"somos um parasita-da-sociedade"... {{/if}}
{{if _.whitebread}}"não comas isso, vai nos matar"... {{/if}}
{{if _.subtweet}}"eles estão a falar pelas nossas costas"... {{/if}}
{{if _.badnews}}"o mundo está a arder"... {{/if}}
{{if _.hookuphole}}"vamos morrer em solidão"... {{/if}}
{{if _.serialkiller}}"eles são um assassino em série"... {{/if}}
{{if _.catmilk}}"gatos não digerem leite"... {{/if}}
{{if _.pokemon}}uma ^merda^ de paródia musical... {{/if}}

h: eu só quero viver minha vida

h: eu só quero ser livre, livre de toda essa... dor.

`bb({eyes:"look_sad"});`

b: Ouve... humano...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Vai ficar tudo bem.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: Como o teu leal lobo-da-guarda, eu vou estar sempre à procura do perigo, e fazer o meu melhor para te manter em segurança.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Eu prometo.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Última aplicação. Instagram. O que tens?

`hong({eyes:"sad"});`

h: São... mais fotos de festas.

`hong({mouth:"sad"});`

h: Todos parecem tão felizes. Livres de preocupações. Livres de ansiedade.

`hong({mouth:"anger"});`

h: Meu Deus, por que não posso ser como eles? Por que não posso ser *normal?*

`bb({eyes:"normal_right"});`

b: Falando em festas, sobre o convite deste fim de semana. Aqui está minha decisão FINAL:

`bb({eyes:"normal"});`

[Devemos ir.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[Devemos ficar longe.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: Dev--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *VAI*

h: *TE*

`hong({body:"2_you"});`

h: F^ODE^R.

(...500)

b: o

(...1500)

`bb({eyes:"wat_2"});`

b: o que?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: Eu vou dizer SIM para aquela festa,

{{if _.act1g=="go"}}
h: NÃO porque tu queres, mas porque *EU* quero.
{{/if}}

{{if _.act1g=="dont"}}
h: Precisamente PORQUE tu não queres que eu vá.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: Tu não me controlas.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: Agora, dá-me licença enquanto eu como a p^orr^a desta sandes deliciosa em paz.

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

[AHHHH VAMOS MORRER](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH TODOS ODEIAM-NOS](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH SOMOS PESSOAS HORRÍVEIS](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH VAMOS MORRER AAAAAAHHHHHHH

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

b: AHHHH TODOS ODEIAM-NOS AAAAAAHHHHHHH

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

b: AHHHH SOMOS PESSOAS HORRÍVEIS AAAAAAHHHHHHH

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

n: PARABÉNS!

(...500)

n: PROTEGESTE AS NECESSIDADES FÍSICAS + SOCIAIS + MORAIS DO TEU HUMANO COM SUCESSO.

n: AFINAL, OLHA COMO ELE ESTÁ GRATO

(...500)

n: AGORA QUE A ENERGIA DELE ESTÁ A ZERO, PODES CONTROLAR AS SUAS AÇÕES DIRETAMENTE

`bb({mouth:"smile", eyes:"normal"});`

n: ESCOLHE O TEU GOLPE FINAL

`bb({mouth:"small_lock", eyes:"fear"});`

n: *ACABA COM ELE*

[{LUTAR: Bate no teu telemovel!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{FUGIR: Enrola numa bola e chora}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: O teu telemovel estava prestes a causar-te um ataque de pânico!

`bb({eyes:"anger"})`

b: O Zuckerberg e compania estão a abduzir a tua saúde mental por lucros capitalistas fáceis!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Castiga o teu telemovel! Destroi-o! Destroi-o!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: MATA MATA MATA MATA MATA MATA MATA MATA MATA MATA MATA MATA MATA MATA MATA MATA MATA MATA MATA--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: O mundo inteiro está cheio de perigos!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Faz como uma tartaru-bola! Enrola-te em auto-defesa!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: ENROLA E CHORA ENROLA E CHORA ENROLA E CHORA ENROLA E CHORA ENROLA E CHORA ENROLA E CHORA ENROLA E CHOR--

(#act1j)

# act1j

`SceneSetup.act1_outro()`
