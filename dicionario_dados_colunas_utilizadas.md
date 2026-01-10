# Dicionario de dados ( Colunas Utilizadas )

Seq. | Nome do Campo | Campo | Tipo / Categoria | Descrição | Características
---- | ------------- | ----- | ---------------- | --------- | ---------------
24 | Sinais clínicos (Febre) | febre | char(1): 1-Sim / 2-Não | Sinal clínico | Campo obrigatório
25 | Sinais clínicos (Mialgia) | mialgia | char(1): 1-Sim / 2-Não | Sinal clínico | Campo obrigatório
26 | Sinais clínicos (Cefaleia) | cefaleia | char(1): 1-Sim / 2-Não | Sinal clínico | Campo obrigatório
27 | Sinais clínicos (Exantema) | exantema | char(1): 1-Sim / 2-Não | Sinal clínico | Campo obrigatório
28 | Sinais clínicos (Vômito) | vomito | char(1): 1-Sim / 2-Não | Sinal clínico | Campo obrigatório
29 | Sinais clínicos (Náusea) | nausea | char(1): 1-Sim / 2-Não | Sinal clínico | Campo obrigatório
30 | Sinais clínicos (Dor nas costas) | dor_costas | char(1): 1-Sim / 2-Não | Sinal clínico | Campo obrigatório
31 | Sinais clínicos (Conjuntivite) | conjuntvit | char(1): 1-Sim / 2-Não | Sinal clínico | Campo obrigatório
32 | Sinais clínicos (Artrite) | artrite | char(1): 1-Sim / 2-Não | Sinal clínico | Campo obrigatório
33 | Sinais clínicos (Artralgia intensa) | artralgia | char(1): 1-Sim / 2-Não | Sinal clínico | Campo obrigatório
34 | Sinais clínicos (Petéquias) | petequia_n | char(1): 1-Sim / 2-Não | Sinal clínico | Campo obrigatório
35 | Sinais clínicos (Leucopenia) | leucopenia | char(1): 1-Sim / 2-Não | Sinal clínico | Campo obrigatório
36 | Sinais clínicos (Prova do laço) | laco | char(1): 1-Sim / 2-Não | Sinal clínico | Campo obrigatório
37 | Sinais clínicos (Dor retroorbital) | dor_retro | char(1): 1-Sim / 2-Não | Sinal clínico | Campo obrigatório
38 | Diabetes | diabetes | char(1): 1-Sim / 2-Não | Doença pré-existente | Campo obrigatório
39 | Doenças hematológicas | hematolog | char(1): 1-Sim / 2-Não | Doença pré-existente | Campo obrigatório
40 | Hepatopatias | hepatopat | char(1): 1-Sim / 2-Não | Doença pré-existente | Campo obrigatório
41 | Doença renal crônica | renal | char(1): 1-Sim / 2-Não | Doença pré-existente | Campo obrigatório
42 | Hipertensão arterial | hipertensa | char(1): 1-Sim / 2-Não | Doença pré-existente | Campo obrigatório
43 | Doença ácido-péptica | acido_pept | char(1): 1-Sim / 2-Não | Doença pré-existente | Campo obrigatório
44 | Doenças auto-imunes | auto_imune | char(1): 1-Sim / 2-Não | Doença pré-existente | Campo obrigatório
60 | Resultado Histopatologia | histopa_n | char(1) | Resultado Exame de Histopatologia | Habilitado apenas se Agravo=Dengue
61 | Resultado Imunohistoquímica | imunoh_n | char(1) | Resultado Exame de Imunohistoquímica | Habilitado apenas se Agravo=Dengue
**_`70`_** | **_`Classificação final`_** | **_`classi_fin`_** | **_`"char(2): 1-Confirmado/2-Descartado/8-Inconclusivo..."`_** | **_`Classificação final do caso após investigação`_** | **_`Campo Obrigatório se data encerramento preenchida`_**

## Campos que podem ser uteis no futuro

Seq. | Nome do Campo | Campo | Tipo / Categoria | Descrição | Características
---- | ------------- | ----- | ---------------- | --------- | ---------------
48 | Resultado IgM Chikungunya S1 | res_chiks1 | char(1): 1-Reagente / 2-Não Reagente / 3-Inconcl / 4-Não realizado | Resultado IgM Soro 1 | Campo Essencial
49 | Resultado IgM Chikungunya S2 | res_chiks2 | char(1): 1-Reagente / 2-Não Reagente / 3-Inconcl / 4-Não realizado | Resultado IgM Soro 2 | Campo Essencial
59 | Sorotipo | sorotipo | char(1): 1-DEN1 / 2-DEN2 / 3-DEN3 / 4-DEN4 | Sorotipo | Obrigatório se Isolamento ou RT-PCR positivo para Dengue
71 | Critério confirmação | criterio | char(1): 1-Lab / 2-Clin/Epi / 3-Clinico... | Critério utilizado para confirmação/descarte | Campo Essencial
73 | Apresentação clínica Chikungunya | clinc_chik | char(1): 1-Aguda / 2-Crônica | Apresentação clínica do caso | Obrigatório se Chikungunya e confirmado
74 | Evolução Do Caso | evolucao | char(1): 1-Cura / 2-Óbito agravo / 3-Óbito outros... | Informar a evolução do caso | Campo essencial
77 | Dengue c/ alarme (Hipotensão) | alrm_hipot | char(1): 1-Sim / 2-Não | Sinal de alarme | Obrigatório p/ Dengue Alarme/Grave
78 | Dengue c/ alarme (Plaquetas) | alrm_plaq | char(1): 1-Sim / 2-Não | Queda abrupta de plaquetas | Obrigatório p/ Dengue Alarme/Grave
79 | Dengue c/ alarme (Vômitos) | alrm_vom | char(1): 1-Sim / 2-Não | Vômitos persistentes | Obrigatório p/ Dengue Alarme/Grave
80 | Dengue c/ alarme (Sangramento) | alrm_sang | char(1): 1-Sim / 2-Não | Sangramento de mucosa/hemorragias | Obrigatório p/ Dengue Alarme/Grave
81 | Dengue c/ alarme (Hematócrito) | alrm_hemat | char(1): 1-Sim / 2-Não | Aumento hematócrito | Obrigatório p/ Dengue Alarme/Grave
82 | Dengue c/ alarme (Dor abdominal) | alrm_abdom | char(1): 1-Sim / 2-Não | Dor abdominal intensa e contínua | Obrigatório p/ Dengue Alarme/Grave
83 | Dengue c/ alarme (Letargia) | alrm_letar | char(1): 1-Sim / 2-Não | Letargia ou irritabilidade | Obrigatório p/ Dengue Alarme/Grave
84 | Dengue c/ alarme (Hepatomegalia) | alrm_hepat | char(1): 1-Sim / 2-Não | Hepatomegalia > 2cm | Obrigatório p/ Dengue Alarme/Grave
85 | Dengue c/ alarme (Líquidos) | alrm_liq | char(1): 1-Sim / 2-Não | Acúmulo de líquidos (derrame) | Obrigatório p/ Dengue Alarme/Grave
87 | Dengue grave (Pulso) | grav_pulso | char(1): 1-Sim / 2-Não | Pulso débil ou indetectável | Obrigatório p/ Dengue Grave
88 | Dengue grave (PA convergente) | grav_conv | char(1): 1-Sim / 2-Não | Pressão Arterial convergente | Obrigatório p/ Dengue Grave
89 | Dengue grave (Enchimento capilar) | grav_ench | char(1): 1-Sim / 2-Não | Tempo de enchimento capilar lento | Obrigatório p/ Dengue Grave
90 | Dengue grave (Insuf. Resp.) | grav_insuf | char(1): 1-Sim / 2-Não | Acúmulo de líquidos com insuf. respiratória | Obrigatório p/ Dengue Grave
91 | Dengue grave (Taquicardia) | grav_taqui | char(1): 1-Sim / 2-Não | Taquicardia | Obrigatório p/ Dengue Grave
92 | Dengue grave (Extremidade frias) | grav_extre | char(1): 1-Sim / 2-Não | Extremidades frias | Obrigatório p/ Dengue Grave
93 | Dengue grave (Hipotensão) | grav_hipot | char(1): 1-Sim / 2-Não | Hipotensão arterial em fase tardia | Obrigatório p/ Dengue Grave
94 | Dengue grave (Hematêmese) | grav_hemat | char(1): 1-Sim / 2-Não | Hematêmese | Obrigatório p/ Dengue Grave
95 | Dengue grave (Melena) | grav_melen | char(1): 1-Sim / 2-Não | Melena | Obrigatório p/ Dengue Grave
96 | Dengue grave (Metrorragia) | grav_metro | char(1): 1-Sim / 2-Não | Metrorragia volumosa | Obrigatório p/ Dengue Grave
97 | Dengue grave (SNC) | grav_sang | char(1): 1-Sim / 2-Não | Sangramento do Sistema Nervoso Central | Obrigatório p/ Dengue Grave
98 | Dengue grave (AST/ALT) | grav_ast | char(1): 1-Sim / 2-Não | AST/ALT > 1.000 | Obrigatório p/ Dengue Grave
99 | Dengue grave (Miocardite) | grav_mioc | char(1): 1-Sim / 2-Não | Miocardite | Obrigatório p/ Dengue Grave
100 | Dengue grave (Consciência) | grav_consc | char(1): 1-Sim / 2-Não | Alteração da consciência | Obrigatório p/ Dengue Grave
101 | Dengue grave (Outros órgãos) | grav_orgao | char(1): 1-Sim / 2-Não | Comprometimento grave de outros órgãos | Obrigatório p/ Dengue Grave
103 | Manifestações Hemorrágicas | mani_hemo | char(1) | Manifestações Hemorrágicas gerais | -
104 | Epistaxe | epistaxe | char(1) | "Se sim |  quais? (Epistaxe)" | -
105 | Gengivorragia | gengivo | char(1) | "Se sim |  quais? (Gengivorragia)" | -
106 | Metrorragia | metro | char(1) | "Se sim |  quais? (Metrorragia)" | -
107 | Petéquias | petequias | char(1) | "Se sim |  quais? (Petéquias)" | -
108 | Hematúria | hematura | char(1) | "Se sim |  quais? (Hematúria)" | -
109 | Sangramento gastrointestinal | sangram | char(1) | "Se sim |  quais? (Sangramento GI)" | -
110 | Prova do laço positiva | laco_n | char(1) | "Se sim |  quais? (Prova do Laço)" | -
111 | Extravasamento plasmático | plasmatico | char(1) | Houve Extravasamento Plasmático | -
112 | Evidenciado | evidencia | char(1) | "Se sim |  Evidenciado Por:" | -
113 | Plaquetas | plaq_menor | char(7) | Plaquetas (Menor valor) | -
114 | Caso de FHD | con_fhd | char(1) | "No caso de FHD/SCD |  especificar" | -
115 | Caso de dengue com complicações | complica | char(1) | Especificar tipo de complicações | -
