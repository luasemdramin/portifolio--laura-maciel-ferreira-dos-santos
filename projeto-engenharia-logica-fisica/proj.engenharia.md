# 🏙️ Sistema de Monitoramento Urbano e Segurança (SMUS)

## 📝 Descrição do Projeto
Este projeto consiste em um conjunto de algoritmos desenvolvidos para análise ambiental e simulação de segurança em ambientes urbanos e internos. Ele integra dois módulos principais: um motor de cálculo de **Nível de Conforto Urbano (NCU)** e **Qualidade do Ar (IQA)**, e um simulador de **Evacuação de Emergência** baseado em lógica de decisão.

Desenvolvido como parte da disciplina de **Inteligência Artificial (2024.1)**, o sistema visa transformar dados brutos de sensores (temperatura, umidade e poluição) em indicadores legíveis, além de modelar o comportamento de agentes em situações críticas de saída de edifícios.

## ⚙️ Funcionalidades Principais
* **Análise de IQA:** Classifica a qualidade do ar de "Boa" a "Perigosa" com base em índices locais.
* **Cálculo de NCU:** Algoritmo matemático que pondera variáveis climáticas e de poluição para gerar uma nota de conforto (0 a 10).
* **Simulador de Evacuação:** Algoritmo de busca e decisão que gerencia recursos (energia), inventário (chaves) e superação de obstáculos em uma rota de fuga.

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python 3.10+
* **Bibliotecas:** `math` (para funções exponenciais e logarítmicas)
* **Paradigma:** Programação Estruturada e Lógica Condicional (`match-case`, `if-elif-else`)

## 📊 Estrutura de Decisão
### Indicadores de Conforto
O sistema utiliza funções matemáticas para normalizar dados:
- **Temperatura:** Modelo de Gauss para conforto térmico ideal em 22°C.
- **Umidade:** Função de penalidade para desvios do patamar de 50%.
- **IQA:** Decaimento exponencial baseado no limite de 200 pontos.

### Lógica de Evacuação
| Estado | Ação |
| :--- | :--- |
| Caminho Livre | Avança para o próximo nó |
| Porta Fechada | Busca chave (retrocede) ou abre (avança) |
| Escada | Incrementa inventário de ação |
| Energia < 0 | Falha na evacuação |

## 🔧 Como Executar
1. Certifique-se de ter o Python instalado em sua máquina.
2. Clone o repositório:
   ```bash
   git clone [https://github.com/seu-usuario/projeto-ia-urbana.git](https://github.com/seu-usuario/projeto-ia-urbana.git)