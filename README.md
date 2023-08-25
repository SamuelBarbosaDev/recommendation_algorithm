# recommendation_algorithm
### Índice

- [recommendation\_algorithm](#recommendation_algorithm)
    - [Índice](#índice)
    - [Contextualização:](#contextualização)
    - [Metodologia Aplicada:](#metodologia-aplicada)
  - [Pré-requisitos para executar o projeto:](#pré-requisitos-para-executar-o-projeto)
    - [Ambiente virtual e Dependências:](#ambiente-virtual-e-dependências)
    - [Crie o arquivo recommender.pkl:](#crie-o-arquivo-recommenderpkl)
    - [Execute a aplicação:](#execute-a-aplicação)


### Contextualização:
O Steam é a plataforma de jogos para PC mais popular do mundo, com mais de 6.000 jogos e uma comunidade de milhões de jogadores. Com uma coleção massiva que abrange desde os grandes blockbusters AAA até os pequenos títulos independentes, as ferramentas de descoberta são um recurso altamente valioso para o Steam.

Dado [o conjunto de dados disponível no Steam](https://www.kaggle.com/datasets/tamber/steam-video-games), a empresa solicitou que criássemos um modelo de recomendação de filtro colaborativo baseado em itens e construíssemos uma API para interagir com esse modelo.

Nosso objetivo é permitir que o usuário insira o nome de um jogo e receba como retorno os 10 jogos mais similares.

**Observação:** Não há uma "avaliação/nota" (*rating*) direta dos jogos, então é necessário calcular uma *rating* implícita usando a seguinte fórmula:

$$r_{\mathbf{ui}} = \frac{hours\ \mathbf{u}\ played\ in\ game\ \mathbf{i}}{total\ hours\ \mathbf{u}\ played}$$

Isso representa o total de horas que o usuário jogou o jogo em relação ao total de horas jogadas em todos os jogos

### Metodologia Aplicada:
A análise foi realizada utilizando o modelo CRISP-DM, o CRISP-DM (Cross Industry Standard Process for Data Mining) é um modelo padrão de processo para projetos de mineração de dados que define um conjunto de fases e tarefas que devem ser executadas para desenvolver soluções de mineração de dados efetivas.

![CRISP-DM](/core/img/CRISP-DM.png)

O modelo CRISP-DM é uma abordagem sistemática e estruturada para a mineração de dados que ajuda as empresas a desenvolver soluções de mineração de dados de maneira eficiente e eficaz, reduzindo o tempo e os custos do projeto.

## Pré-requisitos para executar o projeto:
Abaixo, listarei os requisitos necessários para que o projeto funcione corretamente.

### Ambiente virtual e Dependências:
Criando ambiente virtual:
```
python3 -m venv core/.venv python=3.9.13
```

Entrando no ambiente virtual:
```
source core/.venv/bin/activate
```

Instale as dependências:
```
pip install -r core/requirements.txt
```

### Crie o arquivo recommender.pkl:
Execute o seguinte comando:
```
python3 core/core/train.py
```

### Execute a aplicação:
Execute o seguinte comando:
```
python3 core/core/main.py
```


---
Linkedin: <https://www.linkedin.com/in/samuel-barbosa-dev/> 

E-mail: <samueloficial@protonmail.com>
