# 🌆 Sistemas de Monitoramento Urbano e Simulação de Emergência

## 📝 Descrição do Projeto
Este repositório reúne ferramentas de software voltadas para a análise da qualidade de vida urbana e a validação de protocolos de segurança predial. O projeto integra cálculos avançados de conforto térmico e atmosférico com um motor de simulação de evacuação, permitindo uma visão holística da segurança e bem-estar em ambientes habitados[cite: 6, 7].

O sistema foi estruturado em dois núcleos funcionais:
*   **Análise de Conforto Urbano (NCU):** Processa dados de temperatura, umidade e Índice de Qualidade do Ar (IQA) para gerar métricas de habitabilidade em locais específicos[cite: 6].
*   **Simulador de Evacuação:** Modela a trajetória de um agente em cenários de emergência, considerando obstáculos, gestão de energia e busca por recursos (chaves)[cite: 7].

## 📊 Modelagem Matemática e Lógica

### Índice de Conforto Urbano (NCU)
O cálculo do NCU utiliza uma ponderação de três funções de probabilidade baseadas em variáveis ambientais[cite: 6]:
*   **Temperatura ($pT$):** $$pT(T) = e^{-\left(\frac{T - 22}{10}\right)^2}$$[cite: 6]
*   **Umidade ($pU$):** Determina o conforto hídrico baseado no desvio da umidade ideal (50%)[cite: 6].
*   **Qualidade do Ar ($pIQA$):** Avalia a salubridade atmosférica em uma escala de 0 a 200[cite: 6].

A nota final é calculada pela fórmula:
$$NCU = 10 \times (0.45 \times pT + 0.30 \times pU + 0.25 \times pIQA)$$[cite: 6]

### Lógica de Evacuação Predial
O simulador percorre uma rota pré-definida (Quarto → Corredor → Escada → Sala → Saída Principal), onde o agente deve gerenciar sua energia e inventário para superar bloqueios, como portas trancadas[cite: 7].

## ✨ Funcionalidades
*   **Classificação de IQA:** Identifica automaticamente categorias de "Boa" a "Perigosa"[cite: 6].
*   **Relatórios de Localidade:** Fornece métricas detalhadas para pontos específicos, como Metrô Vila Matilde e Shopping Anália Franco[cite: 6].
*   **Automação de Fuga:** Simula tomadas de decisão em tempo real, incluindo o retorno para buscar itens essenciais[cite: 7].

## 🚀 Tecnologias Utilizadas
*   **Linguagem:** Python 3.x[cite: 6, 7]
*   **Bibliotecas:** `math` (para cálculos exponenciais e logarítmicos)[cite: 6]
*   **Paradigma:** Programação Estruturada e Simulação Lógica

## 🔧 Como Executar
1. Clone este repositório.
2. Certifique-se de ter o Python instalado.
3. Para executar a análise urbana, utilize o arquivo `logica_para_python.py`[cite: 6].
4. Para executar a simulação de emergência, utilize o arquivo `log_python.py`[cite: 7].

---
[Voltar ao início](https://github.com/seu-usuario/seu-usuario)