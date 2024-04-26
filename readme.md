# O que é considerado "ser americano" para o eleitor dos EUA?

![Logo](/assets/logo.jpg)

O projeto consiste na análise dos dados de uma pesquisa que questionava eleitores americanos sobre o que é considerado "ser americano". É um desafio proposto no Clube de Assinaturas da **[Universidade dos Dados](https://universidadedosdados.com)**.

Para realizar o projeto respondendo as perguntas de negócio e fazer a análise gráfico utilizei o Python com as bibliotecas Pandas, Numpy, Seaborn e Matplotlib.

## Sobre os dados

A análise foi realizada utilizando a base de dados de uma pesquisa feita pelo site **[fivethirtyeight](https://projects.fivethirtyeight.com/polls/)**, os dados foram retirados do repositório no **[github](https://github.com/fivethirtyeight/data/blob/master/non-voters/nonvoters_data.csv)**.

## Ferramentas

Utilizei as seguintes ferramentas:

- **Python**: Foi utilizado para realizar a análise exploratória dos dados, tratamento e análise gráfica.

## Perguntas respondidas

### O público da pesquisa

#### **Qual o perfil da amostra analisada? Verifique a distribuição da idade, gênero, raça, nível educacional e salarial.**

**Distribuição do nível educacional:**

Cerca de 39% dos entrevistados possui diploma universitário mas cerca de 59% possuem apenas ensino médio ou menos ou possuem uma graduação não concluída

![Distribuição por nível educacional](/assets/Distribuição_por_nível_educacional.png)

**Distribuição da idade:**

A concentração da idade dos entrevistados está entre 35 e 65 anos.

![Boxplot Idade](/assets/Boxplot_idade.png)

**Distribuição por gênero:**

É bem próximo a quantidade homens e mulheres que responderam a pesquisa, a diferença está em menos de 1%.

![Distribuição por genero](/assets/Distribuição_por_genero.png)

**Distribuição por raça:**

A raça que mais respondeu a pesquisa foi a branca com 63,57%.

![Distribuição por raça](/assets/Distribuição_por_raça.png)

**Distribuição por faixa salarial:**

Existe um equilibrio mas a faixa salarial mais presente é a que ganha entre 75 mil e 125 mil doláres anuais.

![Distribuição por faixa salarial](/assets/Distribuição_por_faixa_salarial.png)

#### **Assumindo que a amostra representa adequadamente a população americana, qual a raça que possui maior poder aquisitivo? E menor?**

Na faixa salarial de 125 mil doláres ou mais, predomina a raça branca com 71% daqueles que responderam a pesquisa. E na faixa de menos de 40 mil dólares com 55% daqueles que responderam também predomina a raça branca. As raças hispanicas e negras, possuem mais pessoas que responderam na faixa daqueles que ganham menos de 40 mil dólares no ano.

Analisando apenas pela raça, a que possui mais pessoas na faixa salarial que recebem de 40 mil dólares ou menos com 72% é a raça negra, que também é que a que possui menos pessoas na faixa salarial de 125 mil dólares com apenas 25% das pessoas que responderam a pesquisa.

![Distribuição_por_faixa_salarial_agrupada_por_raça](/assets/Distribuição_por_faixa_salarial_agrupada_por_raça.png)

#### **Ainda assumindo que temos uma amostra representativa, podemos dizer que nível educacional e poder aquisitivo estão correlacionados?**

As pessoas mais presentes nas faixas salariais mais altas são aquelas que fizeram faculdade, nas faixas salariais mais baixas, estão aquelas com graduação incompleta ou aquelas que fizeram apenas ensino médio ou menos. Ou seja, podemos afirmar que o nível educacional está diretamente relacionado ao poder aquisitivo.

![Distribuição_por_faixa_salarial_agrupada_por_nível_educacional](/assets/Distribuição_por_faixa_salarial_agrupada_por_nível_educacional.png)

### O que é considerado ser um americano?

#### **Um nível educacional maior implica em maior responsabilidade em relação a votar?**

Podemos afirmar que um nível maior de escolaridade implica numa importância maior de votar, cerca de 43% daqueles que considerar muito importante votar são aqueles que possuem um diploma universitário, já aqueles que considerar pouco importante votar, cerca de 59% são aqueles que possuem apenas ensino médio ou menos.

![Importancia_voto_eleições_agrupada_por_nível_educacional](/assets/Importancia_voto_eleições_agrupada_por_nível_educacional.png)

#### **Dentre os não-brancos, o que é mais importante para ser um bom americano: votar em eleições, demonstrar a bandeira americana ou apoiar o exército? Existe uma diferença na preferência de não-brancos de maior poder aquisitivo vs menor poder aquisitivo?**

Para a pergunta de importância do voto, todas as raças acreditam que sejam muito importante votar.

Para a pergunta de demonstrar apoio a bandeira americana, a raça negra e as miscigenadas acreditam que não seja tão importante, apenas a hispânica acredita que seja muito importante.

Com relação ao apoio ao exército, todas as raças acreditam que sejam muito importante apoiar o exército.

![Pergunta_agrupadas_pela_raça](/assets/Pergunta_agrupadas_pela_raça.png)

Para a pergunta de importância do voto, todas as raças não brancas independente da faixa salarial, acreditam que é muito importante votar.

Para a pergunta de demonstrar apoio a bandeira americana, na faixa salarial mais alta, acreditam que não sejam tão importante apoiar o exército e na faixa salarial mais baixa fica bem equilibrado mas predomina aqueles que acham apenas importante o apoio.

Com relação ao apoio ao exército, todas as raças não brancas independente da faixa salarial acreditam que seja muito importante apoiar o exército.

![Pergunta_agrupadas_pela_faixa_salarial](/assets/Pergunta_agrupadas_pela_faixa_salarial.png)

#### **Considerando que respeitar a opinião dos outros (Q2_8) é um indício de tolerância, ao compararmos as gerações de 18-30 anos, 31-50 anos e +51, qual é a mais tolerante e a menos tolerante?**

A maior parte dos entrevistados independente da geração, acreditam que seja importante ou muito importante respeitar a opinião dos outros.

![Respeito_a_opinião_dos_outros_pela_faixa_de_idade](/assets/Respeito_a_opinião_dos_outros_pela_faixa_de_idade.png)

### Escolhas partidárias

#### **Qual escolha partidária, incluindo pessoas sem partido (Q30), possui eleitores mais jovens? E qual possui mais mulheres como apoiadoras?**

Entre todas as faixas etárias, os democratas levam a preferência dos eleitores.

- Entre 18 e 30 anos tem a preferência de 36,3% dos eleitores daquela faixa etária.

- Entre 31 e 50 anos tem a preferência de 31,6% dos eleitores daquela faixa etária.

- Entre eleitores com mais de 50 anos, tem a preferência de 35% dos eleitores daquela faixa etária.

![Escolha_partidária_pela_faixa_de_idade](/assets/Escolha_partidária_pela_faixa_de_idade.png)

#### **Qual o perfil do público sem partido (independent ou no preference), em termos de idade e gênero? E dos republicanos? E dos democratas?**

O público dos partidos independentes são homens com predominância de eleitores acima de 50 anos. Já naqueles que não tem prefêrencia predominam mulheres com a idade predominante acima de 31 anos.

Em ambos partidos, o que pedromina são mulheres e eleitores acima de 50 anos.

![Perfil_do_público_dos partidos_independentes_ou_sem_preferência](/assets/Perfil_do_público_dos_partidos_independentes_ou_sem_preferência.png)

#### **Existe uma correlação entre idade e propensão a votos (voter_category)?**

A categoria que predomina eleitores é a esporádica, com a maiorira daqueles eleitores acima dos 50 anos e a maioria daqueles eleitores entre 31 e 50 anos. Ou seja, não podemos afirmar que existe uma correlação clara entre sempre votar e a idade.

![Perfil_do_público_dos_partidos_republicanos_e_democratas](/assets/Perfil_do_público_dos_partidos_republicanos_e_democratas.png)

### Estratégias Eleitorais

#### **Se você fizesse parte da equipe de marketing do partido republicano, qual público você deveria mirar para atrair mais votos para o partido?**

Fazendo parte da equipe de marketing do partido republicano, direcionaria ações para os públicos:

- Como já possuem grande parte dos eleitores acima dos 50 anos e é o público parecido do partido democrata, eu tentaria atingir aqueles que votam em partidos independentes que são homens com sua maioria acima dos 50 anos e daqueles que não tem preferência que são mulheres acima dos 31 anos para poder aumentar sua base e diferenciar do partido rival.

- Exploraria a importância de votar e o apoio as forças armadas já que grande parte do público independente da raça e da faixa salarial considera muito importante.

- Como possui uma grande massa que vota esporadicamente apenas (já que inclui a mesma faixa etária daqueles que mais votam no partido), exploraria esse público para conseguir somar mais votos convencendo que vale a pena ir votar no partido.
