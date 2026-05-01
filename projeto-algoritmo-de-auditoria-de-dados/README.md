# 🛡️ Algoritmo de Auditoria de Dados de Vendas

## 📝 Descrição do Projeto
Este projeto consiste em um script de automação para auditoria e monitoramento de transações financeiras. O objetivo principal é atuar como uma camada de segurança lógica, identificando discrepâncias em lançamentos de vendas e prevenindo fraudes ou erros operacionais através de protocolos de quarentena e revisão manual.

O sistema processa entradas de vendas, calcula métricas de desempenho e aplica regras de negócio rigorosas para validar a integridade dos dados financeiros, garantindo que anomalias (outliers) sejam devidamente sinalizadas para os auditores.

## ✨ Funcionalidades
*   **Cálculo de Média Transacional:** Processamento automatizado da média de lotes de vendas.
*   **Protocolo de Quarentena:** Bloqueio preventivo do sistema caso a média das operações ultrapasse o limite de segurança estabelecido (R$ 8.000,00).
*   **Detecção de Outliers:** Identificação de vendas individuais que excedem em 5x a média do lote, disparando um alerta de "Revisão Manual"[cite: 1].
*   **Log de Tipagem:** Verificação e exibição dos tipos de dados processados para garantir a precisão matemática[cite: 1].

## 🚀 Tecnologias Utilizadas
*   **Linguagem:** Python 3.x[cite: 1]
*   **Ambiente de Desenvolvimento:** Google Colab / Jupyter Notebook[cite: 1]
*   **Paradigma:** Programação Procedural com foco em Automação

## 📊 Regras de Negócio Implementadas
O algoritmo opera sob as seguintes diretrizes de segurança:
1.  **Limite de Segurança:** Definido globalmente como `8000.00`[cite: 1].
2.  **Quarentena:** Ativada se `media > LIMITE_SEGURANCA`[cite: 1].
3.  **Anomalia Crítica:** Ativada se qualquer venda individual for superior a 500% da média do lote[cite: 1].

## 🔧 Como Executar
1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/seu-usuario/auditoria-vendas.git](https://github.com/seu-usuario/auditoria-vendas.git)