# Grupo51_TechChallenge_fase2
Repositório para o Tech Challenge Fase 2 do Pós Fiap - AI para Devs

# Enunciado do Problema

**Objetivo**

> Este projeto tem como objetivo a solução de um problema relacionado ao **Tech Challenge Fase 2**, do curso de **Pós Graduação de Inteligência Artificial para Desenvolvedores** da Fiap.

**Definição do problema**

- Escolha um problema real que possa ser resolvido por meio de otimização genética.
- Descreva o problema, os objetivos e os critérios de sucesso.

**Testes e Resultados**
 - Realize testes para testar a eficácia do algorítimo.

**Documentação**
Forneça uma documentação completa do projeto incluindo:
- Descrição do problema
- Detalhes da implementação do algorítmo
- Análise dos resultados
- Conclusões.

**Solução Escolhida**

- Escolhemos resolver o problema de **otimização de rotas**, utilizando um algoritmo genético, e que usa um dataset estático, com localização geográfica de todas as cidades do Brasil,
que pode ser aplicado em empresas de **logísticas**, **entregas de produtos**, que são amplamente usados em empresa de diversas áreas, tais como, **e-commerce**, **varejo em geral**, ou em outras cenários, que requeiram algum tipo de otimização complexa.


# Entregável
**Participantes do Grupo 51**

- **RM 355027 - José Hélio Araújo Andrade**

- **RM 356210 - Bernado Guimarães Tinti**

**Links de referências**

- Video de apresentação no Youtube

- [Repositório Github](https://github.com/josehelioaraujo/Grupo51_TechChallenge_fase2/blob/main/Grupo51_TechChallenge_fase2.ipynb)

- [DataSet das cidades do Brasil obtido do Kaggle](https://www.kaggle.com/datasets/gilbertotrindade/cidades-brasileiras?resource=download)

# Fluxograma do Algoritmo Genético
![image](https://github.com/user-attachments/assets/b5a8bd5a-f881-417d-b1bf-58ba2967623e)

Este fluxograma ilustra o processo do nosso algoritmo genético.
   Vamos percorrê-lo passo a passo:

   1. **Início:** O algoritmo começa sua jornada.
   
   2. **Gera População Inicial:** Criamos um conjunto de rotas aleatórias. Pense nisso como criar vários mapas diferentes com rotas entre as cidades.

   3. **Avalia Aptidão dos Indivíduos:** Analisamos quão boa cada rota é, considerando fatores como a melhor distância total entre as cidades.
   
   4. **Verifica Condição de Término:** Checamos se encontramos uma rota boa o suficiente ou se atingimos o número máximo de tentativas.
   
   5. **Seleção:** Se não terminamos, escolhemos as melhores rotas para 'sobreviver' à próxima geração.
   
   6. **Cruzamento:** Combinamos as melhores rotas para criar novas, potencialmente melhores.
   
   7. **Mutação:** Fazemos pequenas alterações aleatórias nas novas rotas para explorar novas possibilidades.
   
   8. **Substitui População Antiga:** As novas rotas substituem as antigas, e voltamos ao passo de avaliação.

   Este processo se repete até encontrarmos uma solução satisfatória ou atingirmos o limite de tentativas.


   # Funções diversas

**Funções usadas no Algorítmo Genético**
- Inicialização do algorítmo genético
- Função a fim de avaliar o Otimizador de Rotas
- Função para criar a matriz de distâncias
- Função para calcular a distância Haversine
- Função para executar o algoritmo genético
- Função para criar a permutação de uma lista
- Implementação do algoritmo de força bruta

**Funções da Interface Visual**
- Função para visualizar a rota no mapa
- Função para plotar o gráfico de convergência
- Função para executar o otimização das cidades selecionadas conforme a quantidade de gerações

**Observações:**

Para o cálculo de distância, usamos o método de **distância Haversine**.

- É um método para calcular a distância entre dois pontos na superfície de uma esfera, como a Terra, usando suas coordenadas de latitude e longitude.

**Em Resumo:**

- É usada para medir distâncias **"great-circle**" na Terra
Leva em conta a curvatura da Terra
Fornece resultados mais precisos que cálculos em um plano 2D
- É comumente usada em **navegação, GPS e aplicações geoespaciai**s
- Usa uma fórmula trigonométrica específica para o cálculo;

- É mais precisa para calcular distâncias na superfície terrestre do que métodos que tratam a Terra como um plano.

- **Fôrmula do cálculo da distância Haversine**:
  
 ![image](https://github.com/user-attachments/assets/eee91e0c-b34a-43d7-977c-f9f74e7f9277)

# Interface visual e interativa

- Função para visualizar a rota no mapa
- Função para plotar o gráfico de convergência

**Ações:**
- Input para digitação da quantidade de gerações
- Widget para seleção de cidades
- Botão 'Executar Otimização'

 ![image](https://github.com/user-attachments/assets/5063a29c-1f80-40e3-96e6-1d63875bf24d)

![image](https://github.com/user-attachments/assets/e4691fa3-4e6f-4ef8-bde9-6c3d070bafbd)

![image](https://github.com/user-attachments/assets/84c90ee9-7386-41e0-a6e8-0b5749559aa0)

# Conclusões

Após realizados os testes com diferentes entradas, diferentes números de cidades, e diferentes algoritmos, é possível concluir que:

- O número de gerações, não fez grande diferença para o algoritmo utilizado, todos se mantiveram no mesmo padrão.

- Além disso foi possível constatar que, o algoritmo de força bruta teve um tempo menor de processamento para os casos com poucas cidades, até 8 cidades.

- Entretanto, o algorítmo genético manteve a constância do tempo de execução mesmo com uma maior quantidades de cidades, dessa forma, para um maior número de cidades o algoritmo genético consegue se sair melhor do que o de força bruta.

 # Recursos adicionais
 
 - [Conversor texto para audio usado na narração do video](https://crikk.com/text-to-speech/portuguese/)
 - **OBS Studio** - usado na gravação do video de apresentação.
 - **DaVinci Resolve** - usado na montagem e edição do video de apresentação.
 - Os arquivos de texto e audio narração e video de apresentação estão na pasta raiz desse repositório.
