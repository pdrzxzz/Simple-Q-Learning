# README - Projeto de Aprendizado por Reforço com Q-Learning

## Visão Geral

Este projeto implementa um algoritmo de Q-Learning para resolver um problema de decisão sequencial em um ambiente estocástico. O ambiente é representado por uma grade com 11 estados, onde o agente deve navegar desde um estado inicial (0) até um dos estados terminais (9 ou 10), que possuem recompensas de -1 e +1 respectivamente.

## Estrutura do Projeto

O código está organizado em um notebook Jupyter com as seguintes seções principais:

1. **Matrizes de Transição**: Define as probabilidades de transição entre estados para cada ação possível (cima, baixo, esquerda, direita).

2. **Funções Auxiliares**:
   - `calc_action_result`: Simula transições estocásticas entre estados
   - `choose_best_action`: Seleciona a ação com maior valor Q
   - `q_update`: Implementa a regra de atualização do Q-Learning
   - `simulate_policy`: Executa a política aprendida
   - `print_policy`: Visualiza a política em formato de grade

3. **Inicialização**: Configura os parâmetros do algoritmo e inicializa a Q-table.

4. **Aprendizado**: Executa o processo de treinamento do Q-Learning.

5. **Simulação**: Testa a política aprendida.

6. **Exercícios Propostos**:
   - Item 1: Experimentos com diferentes valores de alpha e gamma
   - Item 2: Implementação de estratégias de exploração alternativas

## Como Executar

1. Certifique-se de ter instalado:
   - Python 3.x
   - Jupyter Notebook
   - Bibliotecas: numpy, pandas, matplotlib

2. Execute o notebook no Jupyter ou em ambientes como Google Colab.

3. O código pode ser executado célula por célula ou todo de uma vez.

## Parâmetros do Algoritmo

- **Alpha (α)**: Taxa de aprendizado (0.2 no exemplo)
- **Gamma (γ)**: Fator de desconto (0.5 no exemplo)
- **Número de trajetórias**: 5000 no exemplo
- **Recompensas**:
  - Estados não-terminais: -0.04
  - Estado terminal 9: -1
  - Estado terminal 10: +1

## Resultados Esperados

Ao executar o código, você verá:

1. Uma visualização do ambiente (se a imagem estiver disponível)
2. Verificação das matrizes de transição
3. A Q-table final após o treinamento
4. A política aprendida representada graficamente
5. Contagem de visitas a cada par estado-ação
6. Uma simulação da política aprendida

## Personalização

Você pode modificar:
- As matrizes de transição em `T`
- As recompensas em `reward_vector`
- Os parâmetros de aprendizado (ALPHA, GAMMA)
- O número de trajetórias de treinamento

## Contribuição

Contribuições são bem-vindas! Você pode:
- Implementar os exercícios propostos
- Adicionar novas visualizações
- Melhorar a documentação
- Propor extensões ao algoritmo

## Licença

Este projeto está disponível sob a licença MIT.
