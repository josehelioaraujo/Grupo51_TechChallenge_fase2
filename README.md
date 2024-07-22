## **Projeto Tech Challenge Fase 2**

### **Introdução**

Este projeto está relacionado ao **Tech Challenge Fase 2**, do curso de **Pós-Graduação em Inteligência Artificial para Desenvolvedores** da **FIAP**.

### **Definição do Problema**

- Neste projeto, escolhemos abordar o problema de otimização de rotas, que é crucial para empresas de logística e entrega de produtos.
- O objetivo é encontrar a rota mais eficiente para realizar entregas, minimizando custos e tempo, utilizando um algoritmo genético.
- O sucesso será medido pela capacidade do algoritmo em reduzir o tempo total de entrega e os custos operacionais, mantendo a qualidade do serviço.

### **Testes e Resultados**

- Para avaliar a eficácia do algoritmo, serão realizados testes utilizando um dataset estático com a localização geográfica de todas as cidades do Brasil.
- Os resultados serão analisados com base em métricas de desempenho como a redução de tempo de entrega e custos.

### **Documentação**

A documentação do projeto incluirá:

1. **Descrição do Problema**: Detalhamento do problema de otimização de rotas e sua importância.
2. **Detalhes da Implementação do Algoritmo**: Explicação técnica do algoritmo genético utilizado, incluindo pseudocódigo e parâmetros.
3. **Análise dos Resultados**: Discussão dos resultados obtidos nos testes, comparando a eficiência antes e depois da aplicação do algoritmo.
4. **Conclusões**: Reflexão sobre os resultados, destacando os benefícios e possíveis melhorias futuras.

### **Objetivo**

- O nosso projeto, tem o objetivo de resolver o problema de otimização de rotas utilizando um algoritmo genético. Este algoritmo será aplicado a um dataset estático com a localização geográfica de todas as cidades do Brasil.
- A solução é voltada para empresas de logística e entrega de produtos, sendo aplicável em diversos setores como e-commerce, varejo e outros cenários que necessitem de otimização complexa de rotas.

#### **Cenários de Aplicação**

1. **Logística e Entrega de Produtos**:
   - **Problema**: Planejar rotas de entrega que minimizem o tempo e os custos operacionais.
   - **Solução**: Utilizar algoritmos genéticos para determinar a sequência de entregas que otimiza a utilização de recursos e reduz o tempo total de percurso.

2. **Serviços de Transporte Público**:
   - **Problema**: Otimizar as rotas de ônibus ou vans escolares para cobrir todas as áreas de serviço com o mínimo de veículos e tempo.
   - **Solução**: Aplicar algoritmos genéticos para encontrar a melhor rota que maximize a eficiência e minimize os custos operacionais, garantindo que todas as áreas sejam cobertas de maneira eficaz.

3. **Gerenciamento de Frotas de Veículos**:
   - **Problema**: Coordenar a utilização de uma frota de veículos para múltiplas tarefas de maneira eficiente.
   - **Solução**: Utilizar algoritmos genéticos para agendar e otimizar as rotas dos veículos, reduzindo o tempo ocioso e maximizando a produtividade da frota.

4. **Distribuição de Mercadorias em Centros de Distribuição**:
   - **Problema**: Planejar a distribuição de mercadorias de um centro de distribuição para vários pontos de venda.
   - **Solução**: Aplicar algoritmos genéticos para otimizar as rotas de distribuição, minimizando os custos de transporte e melhorando a eficiência do processo logístico.

5. **Gestão de Serviços de Manutenção e Reparos**:
   - **Problema**: Planejar as rotas de técnicos de manutenção para atender vários chamados de serviço em diferentes locais.
   - **Solução**: Utilizar algoritmos genéticos para otimizar as rotas dos técnicos, reduzindo o tempo de deslocamento e melhorando a capacidade de resposta.

- Com essas aplicações, demonstramos a versatilidade dos algoritmos genéticos na resolução de problemas complexos de otimização de rotas, destacando sua relevância em diversos setores da indústria.

# Entregável
**Participantes do Grupo 51**

- **RM 355027 - José Hélio Araújo Andrade**

- **RM 356210 - Bernado Guimarães Tinti**

**Links de referências**

- [Video de apresentação no Youtube](https://www.youtube.com/watch?v=ZDYcPT-mKgA)

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

Este projeto, pode ser utilizado em vários cenários envolve problemas complexos de otimização de rotas, tais como:

- Logística e Entrega de Produtos
- Serviços de Transporte Público  
- Gerenciamento de Frotas de Veículos
- Distribuição de Mercadorias em Centros de Distribuição
- Gestão de Serviços de Manutenção e Reparos

### Reflexão sobre os Resultados

- Os resultados obtidos destacam a eficiência do algoritmo genético em cenários com um grande número de cidades, mostrando-se superior ao método de força bruta para problemas mais complexos.
- Os principais benefícios observados incluem a capacidade de lidar com grandes volumes de dados e a manutenção de um tempo de execução consistente, independentemente do número de cidades envolvidas.

**Pontos de Melhorias**

- Apesar dos resultados positivos, há espaço para melhorias futuras. Algumas sugestões incluem:

- **Aprimoramento dos Parâmetros do Algoritmo**: Ajustar os parâmetros do algoritmo genético, como a taxa de mutação e a seleção de pais, pode melhorar ainda mais o desempenho e a precisão das soluções encontradas.
- **Integração com Dados em Tempo Real**: Incorporar dados em tempo real, como condições de tráfego e clima, pode aumentar a aplicabilidade e a eficácia das soluções de rotas geradas.
- **Hibridização de Algoritmos**: Explorar a combinação de algoritmos genéticos com outras técnicas de otimização, como algoritmos de colônia de formigas ou de enxame de partículas, pode levar a resultados ainda mais robustos.
- **Escalabilidade e Desempenho**: Investigar maneiras de melhorar a escalabilidade do algoritmo para lidar com datasets ainda maiores e mais complexos, garantindo que o tempo de execução permaneça eficiente.

Essas melhorias potenciais podem tornar a solução proposta ainda mais eficaz e aplicável a uma gama maior de problemas de otimização de rotas, beneficiando diversas indústrias e setores.
 # Recursos adicionais
 
 - [Conversor texto para audio usado na narração do video](https://crikk.com/text-to-speech/portuguese/)
 - **OBS Studio** - usado na gravação do video de apresentação.
 - **DaVinci Resolve** - usado na montagem e edição do video de apresentação.
 - Os arquivos de texto e audio narração e video de apresentação estão na pasta raiz desse repositório.
