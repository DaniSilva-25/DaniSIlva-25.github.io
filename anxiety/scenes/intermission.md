# intermission

`Game.clearAll();`

(...2000)

```
_.INTERMISSION_STAGE = _.INTERMISSION_STAGE ? _.INTERMISSION_STAGE : 1;
SceneSetup.intermission(_.INTERMISSION_STAGE);
Game.FORCE_CANT_SKIP = true;
```

(...6000)

```
publish("show_stats");
```

n2: MEDOS NESTA ROUND:

i: #harm# *SE MAGOAR:* {{_.INTERMISSION_STAGE==1 ? _.attack_harm_ch1 : _.attack_harm_ch2}}

i: #alone# *SER DESAMADO:* {{_.INTERMISSION_STAGE==1 ? _.attack_alone_ch1 : _.attack_alone_ch2}}

i: #bad# *SER MÁ PESSOA:* {{_.INTERMISSION_STAGE==1 ? _.attack_bad_ch1 : _.attack_bad_ch2}}


```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n5: (Jogo salvo! Podes sair e continuar depois.)

```
Game.clearAll();
sfx("yelp", {volume:0.5});
```

(...2000)

{{if _.INTERMISSION_STAGE==1}}
(#act2)
{{/if}}

{{if _.INTERMISSION_STAGE==2}}
(#act3)
{{/if}}
