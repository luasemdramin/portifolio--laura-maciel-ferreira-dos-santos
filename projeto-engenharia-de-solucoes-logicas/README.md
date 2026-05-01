# 🏥 Sistema de Classificação de Risco (Triagem)

## 📝 Descrição do Projeto
Este projeto consiste no desenvolvimento da lógica para um sistema de triagem hospitalar automatizado. O objetivo é realizar a classificação preliminar de pacientes com base em sinais vitais e critérios demográficos, auxiliando na priorização do atendimento médico através de níveis de risco (Vermelho, Amarelo e Verde)[cite: 2].

O algoritmo analisa variáveis críticas como pressão arterial, frequência cardíaca (BPM) e temperatura, integrando-as com a idade do paciente para determinar a urgência clínica imediata[cite: 2].

## ⚙️ Lógica de Classificação
O sistema segue um fluxo de decisão binária para categorizar o estado do paciente:
*   **Risco Vermelho (Emergência):** Identificado quando o paciente possui idade superior ou igual a 60 anos, associada a uma pressão arterial igual ou superior a 140/90 mmHg e BPM igual ou superior a 160[cite: 2].
*   **Risco Amarelo (Urgência):** Atribuído quando o paciente apresenta temperatura corporal igual ou superior a 38°C, indicando estado febril[cite: 2].
*   **Risco Verde (Pouca Urgência):** Definido para casos que não se enquadram nos critérios de risco elevado acima[cite: 2].

## 🚀 Estrutura do Algoritmo
*   **Variáveis Utilizadas:** Temperatura (Real), BPM (Real), Pressão (Real) e Idade (Inteiro)[cite: 2].
*   **Entradas de Dados:** O sistema solicita via teclado a pressão, o BPM e a temperatura do paciente[cite: 2].
*   **Processamento:** Utiliza estruturas condicionais compostas para a validação dos parâmetros vitais[cite: 2].

## 📊 Aprendizados e Desafios
Durante o desenvolvimento desta lógica, foram identificados pontos críticos de melhoria e desafios técnicos:
*   **Tradução de Requisitos:** A maior dificuldade encontrada foi a adequação e tradução fiel do fluxograma para a sintaxe de pseudocódigo[cite: 3].
*   **Refinamento de Critérios:** Observou-se a necessidade de especificações mais detalhadas para tornar a classificação de risco ainda mais precisa e específica[cite: 3].

## 🔧 Como Executar (Simulação)
Atualmente, o projeto está em fase de modelagem lógica:
1.  Analise o fluxograma para entender a hierarquia de decisão[cite: 2].
2.  O pseudocódigo pode ser testado em interpretadores de algoritmos compatíveis com a sintaxe "Escreva/Leia"[cite: 2].
3.  Insira os dados vitais conforme solicitado pelo prompt para obter o diagnóstico de risco[cite: 2].

---
[Voltar ao início](https://github.com/seu-usuario/seu-usuario)