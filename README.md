# 🎮 Dados Steam 🎮
Análise de dados retirados da plataforma de venda de jogos online "Steam"

![image](https://i0.wp.com/otageek.com.br/wp-content/uploads/2021/03/Steam-logo-otageek.jpg?fit=810%2C456&ssl=1)

Este reportório analisa uma base de dados da plataforma e analisa-a estatisticamente.

# Contexto
A plataforma "Steam" é uma das maiores plataformas de venda de jogos on-line do mercado digital atual.

Com isto em mente, este reportório tem como objetivo contextualizar os utilizadores e futuros utilizadores da plataforma sobre o conteúdo que poderão encontrar nesta de uma maneira organizada e simples. Pode também ser usado para contextualizar não utilizadores sobre o funcionamento da plataforma e do comércio digital de jogos.

Para atinguir este objetivo, organizámos o reportório através das perguntas mais frequentes dos utilizadores da plataforma, permitindo, em alguns campos, utilizar a perguntam como motor de busca de informação.

# Estrutura

Todos os dados utilizados no reportório são retirados do `steam_games.csv`

O reportório encontra-se organizado através da ordenação aleatória das perguntas mais frequentes.

# Dicionário de Dados

Explicação do significado das colunas de `steam_games.csv`

| Nome | Significado |
| --- | --- |
| `url` | link que direciona para o jogo na plataforma |
| `type` | tipo de ficheiro do jogo |
| `name` | título do jogo |
| `desc_snippet` | descrição breve do jogo disponível na plataforma |
| `recent_reviews` | críticas mais recentes feitas ao jogo |
| `all_reviews` | todas as críticas feitas ao jogo |
| `release_date` | data de lançamento do jogo |
| `developer` | estúdio responsável pela criação do jogo |
| `publisher` | estúdio responsável pela distribuição do jogo |
| `popular_tags` | pequenos descritores do jogo (usualmente em termos específicos da comunidade de jogadores) |
| `game_details` | pequenos descritores usados pela plataforma para facilitar a procura do jogo aos potenciais jogadores do mesmo |
| `languages` | linguagens nas quais o jogo está disponível |
| `achievements` | número de objetivos da plataforma que são possíveis de atingir jogando o jogo |
| `genre` | género(s) do jogo |
| `game_description` | descrição detalhada do jogo |
| `mature_content` | se o jogo contém conteúdo exclusivo para adultos (+18) |
| `minimum_requirements` | especificações mínimas que os computadores dos futuros jogadores do jogo necessitam para o poderem jogar |
| `recommended_requirements` | especificações do computador  recomendadas pelos desenvolvedores do jogo para este ter o máximo de performance |
| `original_price` | preço original/inicial do jogo |
| `discount_price` | preço do jogo após a aplicação de um desconto |

Explicação das colunas adicionadas ao `steam_games.csv`

| Nome | Significado |
| --- | --- |
| `Score` | percentagem de "críticas muito positivas" do jogo |
| `diferenca` | diferença entre os valores encontrados em `original_price` e `discount_price`; este valor é utilizado para calcular a percentagem de desconto do jogo |
| `desc` | cálculo decimal do desconto do jogo |
| `descontoTotal` | cálculo do desconto em percentagem do jogo |
