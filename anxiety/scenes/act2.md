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

s: Mas tu *viste* aquele "artigo de notícias" sobre aquela coisa horrível que aconteceu não-sei-aonde?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: o-oi...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Gente como eu odeio rede de notícias. É tudo sensacionalismo e clickbait.

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: b... bela festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: É verdade, mas essas redes só agem com incentivo. O problema *real* são essas pessoas que clicam no clickbait.

```
publish("act2",["dee",3]);
```

s: Quem iria retweetar um artigo de notícias horrível, fazendo com que todos os seus amigos se sintam mal?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ah, f^od^a né?

(#act2-preamble-end)


# act2-preamble-news2

```
publish("act2",["dee",3]);
```

s: Mas tu *viste* aquele "artigo de notícias" viral na internet?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: o-olá...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Sim, era um artigo falso. Quem é que cai naquilo a ponto de retweetar?

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: b... bela festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Tipo f^oda^-se meu. Sabes, no mínimo abre o Google e pesquisa a respeito antes?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ah, f^od^a-se né?

(#act2-preamble-end)


# act2-preamble-cat

```
publish("act2",["dee",3]);
```

s: Como eu estava a dizer, o Complexo Industrial de Memes explora a vida de gatos.

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: o-olá...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Elabora essa tese.

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: b... bela festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Bem, eu vi alguém retweetar um GIF de um gato a beber leite, ontem.

```
publish("act2",["dee",3]);
```

s: Eles não podem digerir aquela m^erd^a! Quem é que iria retweetar abuso de animais desse calibre?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ugh, f^od^a-se né?

(#act2-preamble-end)


# act2-preamble-tinder

```
publish("act2",["dee",1]);
```

s: Então né, eles nunca me responderam!

```
publish("act2",["dee",0]);
publish("act2",["party_hong","next"]);
```

h2: o-olá....

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Isso apesar de que vocês os dois deram match no Tinder?

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: b... bela festa...

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

s: É, nem sei! Sei lá, será que acharam que eu era um assassino em série ou algo do tipo? Tanta coisa maluca.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ah, f^od^a-se né?

(#act2-preamble-end)


# act2-preamble-hookuphole

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: É, nem sei! Talvez eles acham que sexo casual não é preenchimento suficiente para o coração deles?

s: Tipo, para de ser tão idiota! Abre a mente, depois abre essas pernas!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Ah, f^od^a-se né?

(#act2-preamble-end)


# act2-preamble-pokemon

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: É, nem sei! Nem era tão atraente assim, mas eu comia!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Temos que Pegar!™

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

n: ROUND 2: *FIGHT!*

[Oh não, todos eles nos odeiam!](#act2a_social)

[Tu estás *de olho* naquela ruiva?](#act2a_perv)

[Oi, vamos conversar sobre o sentido da vida.](#act2a_meaning)

# act2a_social

`bb({eyes:"sad"})`

b: Estamos a acabar com o clima desta festa por sermos quadrados e tristes!

`bb({eyes:"shock", body:"two_up"})`

b: Estamos a matar a vibe! Cometendo vibe-cídio de primeiro grau!

`bb({eyes:"normal", body:"normal"})`

b: Humano, temos que sair *agora* antes que--

```
_.a2_first_danger = 'social';
_.a2_attack_1 = "alone";
```

(#act2b)

# act2a_perv

`bb({eyes:"suspect"})`

b: Eles são mais atraentes que nós, isso significa que se sequer *olharmos* para aquela pessoa então--

`bb({eyes:"shock", body:"two_up"})`

b: SOMOS ESQUISITOIDES

`bb({body:"normal"})`

b: Somos esquisitos, objetificadores, terríveis tarados maus maus ma--

```
_.a2_first_danger = 'perv';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2a_meaning

`bb({body:"one_up", eyes:"normal_r"})`

b: No final de tudo, o que é que podemos fazer que realmente importará? 

`bb({body:"normal", eyes:"sad"})`

b: Contribuir para a humanidade? Todos os grandes trabalhos voltam ao pó como observado em Ozymandias. Amor? A morte sempre separará.

`bb({eyes:"sad_r"})`

b: E olha quanta morte que tem por aí! *Nós* vamps morrer. *Todos que amamos* vão morrer.

`bb({eyes:"shock", body:"two_up"})`

b: F^oda^-se, a Segunda Lei da Termodinâmica significa que até nosso *universo* vai morrer!

`bb({eyes:"suspect", body:"normal"})`

b: Mas "ora, a morte faz com que apreciemos a vida"? Isso é tipo, dizer que escravidão é boa porque faz com que apreciemos a liberdade!

`bb({body:"one_up"})`

b: Mas "ora, precisas de inventar o teu próprio significado"? Isso é coisa que cultistas e teoristas da conspiração dizem!

`bb({eyes:"shock", body:"two_up"})`

b: A vida não tem significado, a morte não tem significado, até *significar* não tem significado! O que uma alma mortal deveria estar faz--

```
_.a2_first_danger = 'meaning';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2b

`bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"suspect"})`

b: Hum... estás a ouvir, humano?

`bb({eyes:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"shock", mouth:"small_talk", body:"chest", MOUTH_LOCK:true})`

b: *GASP*

`bb({mouth:"small_talk"})`

b: EU TENHO DE TE AVISAR DE...

[*Mais* do mesmo perigo!](#act2b_louder)

{{if _.a2_first_danger=="social"}}
[Um perigo social *diferente*!](#act2b_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[Um perigo social *diferente*!](#act2b_different_moral)
{{/if}}

[Estás a ignorar-me! Isso é perigoso!](#act2b_ignore)

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

b: EMOÇÕES SÃO CONTAGIOSAS! ENTÃO SE NÃO FORES EMBORA, VAIS INFETAR TODOS COM A TUA DOENÇA MENTAL! 

b: Vais criar um surto letal de SÍNDROME DE TRISTEZA QUADRADA

`bb({eyes:"suspect", body:"normal", mouth:"normal"})`

b: Temos de sair daqui e colocarmo-nos em quarentena para sempre, num quarto com Netflix e acesso a tele-entrega!

```
_.a2_second_danger = 'netflix';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "uma quarentena";
```

(#act2c)

# act2b_louder_perv

`bb({eyes:"suspect", body:"two_up", mouth:"normal"})`

b: NÃO SEJAS ALGUÉM ESQUISITO. É CONTRA A LEI!

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

b: Lei dos Esquisitoides, Seção 74.5: (1) Qualquer sujeito que ficar encarando (a) aqueles ombros definidos (b) aquele ^cu^ redondo (2) será, a partir do tal, conhecido como

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: "UM MONSTRO TARADO NOJENTO E IMUNDO"

```
_.a2_second_danger = 'law';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "a lei";
```

(#act2c)

# act2b_louder_meaning

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: Na realidade, mesmo que tu encontres um propósito nobre na vida, *ainda podes* arruinar tudo!

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Alfred Nobel queria paz mundial e que diferentes culturas se entendessem. Então, ele decidiu facilitar o conceito de viagens.

`bb({eyes:"normal_r"})`

b: Ele precisava de uma maneira de criar túneis de comboio de forma barata e rápida. Daí, ele inventou um novo material chamado "dinamite"...

`bb({body:"one_up", eyes:"normal"})`

b: que foi utilizada na Primeira Guerra Mundial para MATAR MILHÕES DE PESSOAS

`bb({body:"two_up", eyes:"shock"})`

b: É O EFEITO BORBOLETA, HUMANO! SABES QUANTAS PESSOAS ESTÁS A MATAR ACIDENTALMENTE AGORA MESMO

```
_.a2_second_danger = 'butterfly';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "Primeira Guerra Mundial";
```

(#act2c)

# act2b_different_social

`_.a2_first_choice = "different"`

`bb({eyes:"normal_r", body:"point", mouth:"normal"})`

b: Na realidade, sabes o que é pior que ninguém gostar de ti? *Todos* gostarem de ti.

`bb({body:"one_up", eyes:"suspect", mouth:"normal"})`

b: Quero dizer, tornar-se um *daqueles* malucos de festa em busca de prazer.

`bb({body:"normal", mouth:"small"})`

b: Uma vida rasa com amigos rasos, que apenas conhecem o "tu" raso.

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Humano, precisamos fugir destes zombies-do-prazer antes que nos tornemos um deles!

```
_.a2_second_danger = 'zombies';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "zombies";
```

(#act2c)

# act2b_different_moral

`_.a2_first_choice = "different"`

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Pessoas estão a morrer à fome e de genocídio *agora mesmo*, e simplesmente estamos a festejar!

`bb({body:"point", eyes:"closed", mouth:"small"})`

b: Uma pessoa sábia uma vez disse, "A única coisa necessária para o triunfo do mal é que as pessoas boas não façam nada."

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: NÃO ESTAMOS A FAZER NADA.

`bb({mouth:"small"})`

b: AO FESTEJAR, ESTAMOS A AJUDAR O *HITLER*.

```
_.a2_second_danger = 'hitler';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "Hitler";
```

(#act2c)

# act2b_ignore

`_.a2_first_choice = "ignore"`

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Achas que estás em segurança por retirar as baterias do detector de monóxido de carbono?

`bb({eyes:"suspect_r"})`

b: Nem vais sentir o cheiro do veneno! Simplesmente vais adormecer, e então vais--

`bb({body:"scream_c_1"})`

b: MOOOOORREEEEEEEEEER

```
_.a2_second_danger = 'ignore';
_.a2_attack_2 = "harm";
_.a2_hoodie_callback = "monóxido de carbono";
```

(#act2c)

# act2c

```
hong({body:"ignore_sweat"});
bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true});
```

b: ...

`bb({eyes:"happy", mouth:"smile", body:"chest"})`

b: Ah que bom, humano! Acho que já me podes me ouvir denovo!

`bb({eyes:"closed", body:"point"})`

b: AGORA VOU TE ALERTAR DE...

{{if _.a2_first_choice=="louder"}}
[*Ainda mais* do mesmo perigo!](#act2c_louder)
{{/if}}

{{if _.a2_first_choice!="louder"}}
[*Mais* do mesmo perigo!](#act2c_louder)
{{/if}}

{{if _.a2_first_danger=="social"}}
[Um perigo social *diferente*](#act2c_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[Um perigo social *diferente*](#act2c_different_moral)
{{/if}}

[Verificaste esse ponche antes de o beberes?](#act2c_punch)

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

b: Na realidade, Netflix & tele-entrega não é quarentena o suficiente! Ainda poderiamos infetar o homem da entrega!

`bb({body:"one_up", mouth:"small"})`

b: Temos de ir para os territórios Canadenses de Yukon, e receber nossa tele-entrega por drones!

`bb({body:"two_up", mouth:"normal"})`

b: E então eles teriam que esterilizar o drone para livrá-lo de nossos GERMES DE TRISTEZA QUADRADA

`_.a2_attack_3 = "alone";`

`_.a2_hoodie_callback = "uma quarentena";`

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

b: O sujeito "MONSTRO TARADO NOJENTO E IMUNDO" será sentenciado a 72 horas em um daqueles pelourinhos medievais para humilhação em praça pública.

b: exceto no caso deles secretamente *gostarem* desse tipo de coisa.

`bb({body:"scream_a_1"})`

b: por serem UM MONSTRO TARADO, NOJENTO, E IMUNDO

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "a lei";`

(#act2d)

# act2c_louder_butterfly

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: EFEITO BORBOLETA! Estás a usar um copo plástico não bio-degradável?

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: BOOM, UM ATERRO COMEÇA A VAZAR VENENO E MATA UMA CRIANÇA

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: Estás suando e o teu coração está a palpitar agressivamente?

`bb({body:"scream_a_1"})`

b: BOOM, ACABASTE DE FALIR O SISTEMA PÚBLICO DE SAÚDE E MILHÕES MORREM EM SEGUIDA

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "o efeito borboleta";`

(#act2d)

# act2c_louder_zombies

`bb({body:"normal", mouth:"small", eyes:"angry"})`

b: Estes zombies-do-prazer vão partir para cima de ti a murmurar,

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: GOSTOS. GOOOOOOSTOOOS.

`bb({body:"scream_a_1"})`

b: E então eles vão TE MORDER e transformar-te num ACÉFALO "DOS BROTHER" ou numa P^UT^A SEM FUTURO!

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "zumbis";`

(#act2d)

# act2c_louder_hitler

`bb({body:"scream_a_1"})`

b: OS NAZIS ESTÃO A MARCHAR QUE NEM PATOS PARA AS RUAS AGORA MESMO

`bb({body:"one_up", mouth:"smile", eyes:"happy"})`

b: A dizer, *ainda bem que aquela 'gente boa' foi se preocupar com coisas tipo 'relaxar' e 'auto-ajuda'!*

`bb({body:"point", mouth:"smile", eyes:"happy_r"})`

b: *Agora o país é o nosso quarto, do reich que deveria ser!*

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "Hitler";`

(#act2d)

# act2c_louder_ignore

`bb({body:"normal", mouth:"normal", eyes:"normal_r"})`

b: Pensando nisso, será que este prédio *sequer tem* um detector de monóxido de carbono?

`bb({body:"two_up", mouth:"small", eyes:"normal"})`

b: E se estivermos a ser envenenados *AGORA MESMO*?

`bb({body:"scream_a_1"})`

b: NEM VEREMOS A MORTE SE APROXIMAR. SIMPLESMENTE DEIXAREMOS DE EXISTIR PARA SEMPRE E SEMPRE E SE--

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "monóxido de carbono;`

(#act2d)

# act2c_different_social

`bb({body:"normal", mouth:"normal", eyes:"sad"})`

b: E se formos, simplesmente, *fundamentalmente incapazes* de sermos amados, ou de amarmos alguém?

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: E se algo, simplesmente, *irreversivelmente* partiu-se dentro de nós, um longo tempo atrás? Ou se este algo *nunca existiu* dentro de nós, para começo de história?

`bb({body:"scream_a_1"})`

b: AHH SOMOS TÃO PARTIDOS!! TÃO PARTIDOS TÃO PARTIDOS TÃO PARTIDOS--

`_.a2_attack_3 = "alone";`

(#act2d)

# act2c_different_moral

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: E se formos, simplesmente, *fundamentalmente podres?*

`bb({body:"one_up", eyes:"sad"})`

b: Outras pessoas tem um instinto interno de fazer o bem, enquanto nós fazemos o bem apenas se nos sentirmos culpados ou envergonhados, sequer isso.

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: E se for da nossa natureza magoar os outros? E se não for possível fazer nada *além* de ser um peso para aqueles em nossa volta?

`bb({body:"scream_a_1"})`

b: AHH SOMOS TÃO PARTIDOS!! TÃO PARTIDOS TÃO PARTIDOS TÃO PARTIDOS --

`_.a2_attack_3 = "bad";`

(#act2d)

# act2c_punch

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Não estou a ser irracional. Tem gente que *realmente* mete "boa noite cinderela" em taças de ponche. Isso é uma coisa real, que acontece.

`bb({eyes:"suspect"})`

b: Humano, dói-te a cabeça? Os teus membros estão dormentes? Eu acho que estamos a morrer.

`bb({body:"scream_a_1"})`

b: AHHH ESTAMOS A MORRER! ESTAMOS A MORRER ESTAMOS A MORRER ESTAMOS A MORR-

`_.a2_attack_3 = "harm";`

`_.a2_hoodie_callback = "taças de ponche";`

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

h: F^ODA^-SE!

h: C^ARALH^O FILHO DE TRINTA MIL P^UTA^S

`bb({body:"two_up", mouth:"smile", eyes:"happy"});`

b: Elá, humano! Estou tão feliz que podes ouvir-me denovo!

`bb({body:"normal", mouth:"small", eyes:"sad"})`

b: Por que é que estavas a ignorar-me?

`hong({body:"facepalm"})`

h: Santa c^on^a do assobio, seu imbecil total.

`hong({body:"facepalm_2"})`

h: Sabes aquele conto dos americanos nativos?

h: "Existem dois lobos dentro de ti, um é a esperança, o outro o desespero, qual lobo ganha? Aquele que o alimentares."

```
hong({body:"facepalm_3"});
bb({eyes:"normal"});
```

h: Eu estava tentar fazer com que *morresses de fome*, seu filho da ^puta^ sádico!

`hong({body:"smile", mouth:"smile"})`

h: F^oda^-se, vou usar afirmações positivas ao invés disso.

h: *Eu sou amável. Eu sou do bem. Eu sou inteligente. Eu sou apreciável. Eu sou especial.*

`bb({eyes:"suspect"});`

[Ui, quanto narcisismo!](#act2d_narcissist)

[Sabes que afirmações assim foram *desprovadas?*](#act2d_disproven)

[pelamordedeus não atribuas mentiras à indigenas](#act2d_racist)

# act2d_disproven

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: De facto, essas afirmações *saem pelo ^cu^* de pessoas de baixa auto-estima! 

`bb({body:"one_up", mouth:"small", eyes:"normal"})`

b: Foi um estudo bem projetado – um teste controlado e unánime, o experimentador foi impedido de ver quem estava em qual grupo.

`bb({body:"two_up", mouth:"small", eyes:"normal_r"})`

b: Resultados: se já tinhas baixa auto-estima, ser ordenado a repetir afirmações como essas fazem-te sentir *pior* do que se não tivesses dito nada!

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Wood 2009, Psychological Science. Pesquisa lá no Google Scholar, humano,

`bb({body:"scream_b_1"})`

b: E PARA DE ESPALHAR PSEUDOCIÊNCIA

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_narcissist

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: *Precisas* ver, humildemente, as tuas próprias falhas para poderes crescer como alguém!

`bb({body:"two_up", eyes:"suspect"})`

b: Não podes simplesmente usar um desodorizante de ar num quarto cheio de mofo! Cobrir as tuas falhas fará ficares pior a longo prazo.

`bb({body:"chest", mouth:"smile", eyes:"closed"})`

b: Felizmente, eu, como o teu leal lobo-da-guarda, posso te avisar das tuas falhas. E no momento, parece ser-

`bb({body:"scream_b_1"})`

b: TUDO. TUDO ESTÁ ERRADO

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_racist

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Nativos são *pessoas reais*. Não são "selvagens nobres" para meter numa conversa, de modo que o teu conselho de bolachas da sorte pareça mais *exótico*.

`bb({eyes:"suspect_r"})`

b: Estás a reduzir pessoas individuais e culturas complexas ao transformá-los num cartão de mensagem. Isso chama-se "racismo benevolente"! 

`bb({body:"scream_b_1"})`

b: PARA DE SER RACISTA, IMBECIL DE OLHOS PUXADOS

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2e

h: ^CABRÃO^ DE ^MERDA^.

`hong({body:"yell", mouth:"yell"})`

h: Queres saber? Tu és *irracional*.

h: Todos sabem que emoções são irracionais! Especialmente o medo!

`hong({body:"facepalm_2"})`

h: Tu és um resto evolucionário inútil, como meu apêndice, ou dentes de siso!

`hong({body:"yell", mouth:"yell"})`

h: F^oda^-se, esta metáfora do lobo é doida! Tu és simplesmente um monte de átomos na minha cabeça.

`hong({body:"cross", mouth:"cross"})`

h: Então porque é que *eu* devia ouvir as palavras de um imprestável, irracional, inexistente pedaço de m^erd^a como tu?!

`bb({eyes:"sad", MOUTH_LOCK:true})`

b: ...

[Fogo, humano. Isso é bem rude.](#act2e_hurtful)

[Eu sou um sentimento. Sentimentos são válidos.](#act2e_valid)

[Humano, *ambos* somos "apenas átomos."](#act2e_rational)

# act2e_hurtful

`bb({body:"chest"})`

b: Eu sou *parte* de ti, sabes. Quando dizes isso, estás a magoar-te *a ti próprio*.

`bb({body:"scream_a_1"})`

b: Por que é que estás a bater-te, humano? PARA DE TE BATER.

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

b: Os teus maiores motivadores são dopamina, as tuas maiores alegrias são seratonina.

`bb({body:"one_up"});`

b: As tuas memórias são pesos sinápticos, a tua razão são sinais elétricos propícios a falha.

`bb({eyes:"normal", body:"normal"});`

b: Então se eu sou "apenas átomos" significa que *Eu sou* irracional... isso significa que *tu* é irracional!

`bb({body:"two_up", eyes:"shock"});`

b: E se *ambos* somos irracionais, então nunca vamos descobrir como ser felizes e íntegros!

`bb({body:"scream_a_1"})`

b: AHH SOMOS TÃO PARTIDOS!! TÃO PARTIDOS TÃO PARTIDOS TÃO PARTIDOS--

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

b: Espera aí... "eles" dizem que sentimentos são válidos, e que tu deves sempre aceitar as tuas emoções.

`bb({eyes:"suspect_r"});`

b: Mas "eles" também dizem que emoções são irracionais, que não se deve confiar nelas.

`bb({eyes:"angry"});`

b: Ai ai, "eles" estavam a mentir-nos este tempo todo!

`bb({body:"scream_a_1"})`

b: "ELES" ALIMENTARAM-NOS COM CONTRADIÇÕES PARA NOS TORNAR DEPENDENTES NO COMPLEXO INDUSTRIAL DE AUTO-AJUDA

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

h: Eu odeio isso. Deus isso dói tanto eu *odeio* isso.

h: Eu não consigo te aturar. Eu não consigo te ignorar. Eu não consigo brigar contigo. 

`bb({eyes:"suspect"});`

h: Não importa o que eu faça, não consigo me livrar de t--

`bb({body:"cry_1"});`

b: Bem, talvez tu *NÃO DEVERIAS* LIVRAR DE MIM

`bb({body:"cry_2"});`

b: Como é que achas que *EU* me sinto, humano?!

`bb({body:"cry_4", mouth:"cry", eyes:"cry"})`

b: Estou a dar o meu melhor para ser o teu cão-de-guarda, mas tu só me vês como um lobo mau!

b: Então eu tento ainda mais avisar-te sobre o perigo! *Mais* perigos! Perigos *diferentes*!

`bb({eyes:"cry_2"})`

b: Mas não importa o quanto eu tente proteger-te, *ainda* achas que sou teu inimigo!

`bb({body:"cry_5"});`

b: O que é que eu estou a fazer de errado?!

`bb({body:"cry_2"});`

b: Eu *sei* que eu não estou a fazer um bom trabalho. Mas estou *a tentar*, humano!

`bb({body:"cry_3"});`

b: ...Estou a tentar.

`bb({body:"cry_6", mouth:"right", eyes:"cry_r_1"});`

b: Não tens que prestar atenção aos meus avisos, ou concordar comigo, ou sequer *gostar* de mim.

`bb({eyes:"cry_r_2"});`

b: Eu simplesmente... quero que sejas paciente comigo.

`bb({eyes:"cry_r_3"});`

b: Só quero que sentes comigo por um tempo, e não dar as costas para mim e--

```
bb({eyes:"cry_r_4"});
hong({body:"listen"});
```

r: Oi.

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

r: Parece que te perdeste numa briga interna, jovem.

```
publish("act2",["party_hunter",3]);
publish("act2",["party_hong",13]);
```

h2: Estava tão óbvio assim?

```
publish("act2",["party_hunter",4]);
publish("act2",["party_hong",14]);
```

r: Estavas, uh, falando com a tua camisola sobre {{_.a2_hoodie_callback}} ou algo assim.

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

h2: meu deus sou uma confusão.

```
publish("act2",["party_hunter",7]);
publish("act2",["party_hong",18]);
sfx("squeak");
```

r: Ei. Não és só tu, colega. Ansiedade é algo super comum.

```
publish("act2",["party_hunter",5]);
publish("act2",["party_hong",19]);
```

{{if _.act1_ending=="fight"}}
r: Ui, ontem mesmo, ouvi que alguém teve um ataque nervoso na faculdade e partui o próprio telemovel
{{/if}}

{{if _.act1_ending=="flight"}}
r: Ui, ontem mesmo, ouvi que alguém se enrolou numa bola e chorou em público!
{{/if}}

```
publish("act2",["party_hunter",2]);
```

r: Ouve: Sei bem como é ter um animal dentro da tua cabeça.

```
publish("act2",["party_hunter",8]);
```

r: Todos *aqui* sabemos. É por isso que fazemos estas festas todos os fins de semana, para esquecer das nossas preocupações, daquele animal.

```
publish("act2",["party_hunter",9]);
publish("act2",["party_hong",20]);
```

h2: mas a minha ansiedade...

```
publish("act2",["party_hunter",2]);
publish("act2",["party_hong",21]);
```

r: Não te preocupes, jovem. Eu já fui como tu. Mas então, eu encontrei um pequeno truque para fazer com que aquela voz negativa se calasse para sempre...

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

r: A minha receita especial. É um pouquinho mais forte que... bem, qualquer coisa legalizada.

```
publish("act2",["party_hunter",12]);
publish("act2",["party_hong",24]);
```

r: Enfia lá para dentro, c^aralh^o!

```
hong({body:"hold"});
bb({body:"normal", mouth:"small", eyes:"wat"});
Game.clearText();
Game.WORDS_HEIGHT_BOTTOM = -1;
publish("act2-out-3");
publish("hp_show");
```

(...3500)

[Ai meu Deus.](#act2g_1) `Game.OVERRIDE_CHOICE_LINE=true`

[Isso é uma péssima forma de lidar com as coisas.](#act2g_2) `Game.OVERRIDE_CHOICE_LINE=true`

[Não aceites bebida de estranhos.](#act2g_3) `Game.OVERRIDE_CHOICE_LINE=true`

# act2g_1

b: A--

(#act2g)

# act2g_2

b: I--

(#act2g)

# act2g_3

b: N--

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

h: Mmm, que bebida tão deliciosa!

h: Um sabor da cabeça-aos-pés de "cala a boca", com um pozinho de "nunca sintas nada denovo"!

b: Isso é mau, humano. Isso é muito, muito mau.

[Isso é *exatamente* como vício começa.](#act2h_opt1) `Game.OVERRIDE_CHOICE_LINE=true`

[Eu *sabia* que a anfitriã era uma confusão por dentro!](#act2h_opt3) `Game.OVERRIDE_CHOICE_LINE=true`

[E, eles podem ter drogado isso aí!](#act2h_opt2) `Game.OVERRIDE_CHOICE_LINE=true`


# act2h_opt1

b: Isso é *exat*--

(#act2h)

# act2h_opt2

b: E, eles pod--

(#act2h)

# act2h_opt3

b: Eu *sabia* qu--

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

h: Delicioso, *e* mais barato que terapia!

b: HUMANO POR FAVOR PARA

h: Hehehe!

h: E o que é que *tu* pretendes fazer a respeito, ^cabrão^?

b: Desculpa, humano.

b: Eu vou ter de usar meu GOLPE ESPECIAL

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

h: Que m^erd^a?

h: Vais ladrar mais *palavras* estúpidas pra cima de mim para--

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

h: QUE ^CARALHO^ FOI AQUILO???

b: Desculpa. Eu tive que mostrar como seriam as consequências.

{{if _.SPECIAL_ATTACK=="harm"}}
h: EU PUDE *VER* O MEU PRÓPRIO CORPO. EU PUDE *SENTIR* A SENSAÇÃO DE BATER A BOTA.
{{/if}}

{{if _.SPECIAL_ATTACK=="alone"}}
h: EU PUDE *VER* O OLHAR DE DESGOSTO DE TODOS. EU PUDE *OUVIR* AS COISAS HORRÍVEIS QUE DISSERAM.
{{/if}}

{{if _.SPECIAL_ATTACK=="bad"}}
h: EU PUDE *OUVIR* AS COSTELAS QUEBRANDO. EU PUDE *SENTIR* O GOSTO DE SANGUE NO AR.
{{/if}}

b: Desculpa, humano.

n: *ACABA COM ELE*

[{LUTAR: Dar um soco na anfitriã.}](#act2j_fight) `Game.OVERRIDE_CHOICE_LINE=true`

[{FUGIR: Vamos sair daqui.}](#act2j_flight) `Game.OVERRIDE_CHOICE_LINE=true`

# act2j_fight

`bb({ eyes:"angry" });`

b: Aquela psicopata estava a tentar apoderar-se de ti.

b: Tentaram te corromper, te confundir para ficares que nem eles!

`bb({ body:"yell_angry_1" });`

b: Dá um soco naquela imbecil! Apagua ela de vez!

`bb({ body:"final_1" });`

b: PORRADA PORRADA PORRADA PORRADA PORRADA PORRADA PORRADA --

`_.a2_ending = "fight";`

(#act2k)

# act2j_flight

b: Eu *sabia* que todos estas pessoas eram doentes. Eles apagam a dor com coisas horríveis!

`bb({ body:"yell_1" });`

b: E eles estão a tentar enganar-te para fazeres a mesma coisa! Eles estão a corromper-te! Temos que sair daqui!

`bb({ body:"final_1" });`

b: SAI SAI SAI SAI SAI SAI SAI SAI SAI SAI --

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

r: Estás bem, jovem?

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

r: Tu...

```
publish("act2",["party_hunter",23]);
publish("act2",["party_hong",35]);
publish("act2",["dee",5]);
publish("act2",["dum",5]);
music('party1', {volume:0.6, fade:6});
```

r: és *selvagem*.

r: Eu gosto disso. Vem cá para a semana, jovem.

```
publish("act2",["party_hunter",19]);
publish("act2",["party_hong",36]);
```

h2: ok xau, ciao, adios, au revoir

r: O animal talvez tenha ganho por hoje, mas volta, vou misturar algo ainda mais forte só pra ti!

h2: goodbye, sayōnara, auf wiedersehen, zài jiàn, shalom

r: Eu e tu, jovem, vamos mostrar aquela besta quem manda!

(#act2k_end)

# act2k_flight

`publish("act2",["party_hong",36]);`

h2: ok desculpa eu tenho que tocar daqui

`publish("act2",["party_hunter",16]);`

r: *Que c^aralh^o*. O animal ganhou hoje, não é?

`publish("act2",["party_hunter",15]);`

h2: não não, eu só, hã, tenho que correr na maratona. bem rápido.

`publish("act2",["party_hunter",19]);`

r: Vem cá para a semana, jovem. Vou misturar algo ainda mais forte só pra ti.

h2: ok obrigado tenho que ir indo irei

r: Eu e tu, jovem, vamos mostrar para aquela besta quem manda!

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

b: Humano! estás bem?!

```
publish("act2", ["act2_end","next"]);
```

b: Meu Deus, essa foi por *pouco.* Nós realmente poderiamos ter--

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

h: Eu vou voltar cá para a semana.

h: A próxima vez que brigarmos, não só vou *derrotar-te*...

h: Eu vou te *matar*, c^aralh^o.

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
