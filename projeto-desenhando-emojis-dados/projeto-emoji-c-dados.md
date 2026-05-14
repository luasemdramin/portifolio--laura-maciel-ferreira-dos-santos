# 🎨 Processamento Digital de Ativos e Bibliotecas Multimídia

## 📝 Descrição do Projeto
Este projeto foi desenvolvido como parte de estudos em **Inteligência Artificial e Processamento de Dados (2024.1)**. Ele foca na manipulação de estruturas de dados complexas para ativos digitais, abrangendo desde a inversão de frequências sonoras em bibliotecas musicais até o processamento de matrizes de pixels para renderização de imagens e emojis.

O sistema demonstra a aplicação prática de algoritmos para:
* **Manipulação de Frequências:** Inversão de sequências harmônicas em dicionários aninhados.
* **Processamento de Imagem:** Algoritmos de sombreamento (shadowing) através da manipulação de canais RGB.
* **Gestão de Assets:** Organização e processamento de strings e emojis em playlists temáticas.

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python 3.10
* **Bibliotecas:** * `Matplotlib`: Para visualização e renderização de matrizes de pixels.
* **Ferramentas:** Google Colab, Jupyter Notebook

## 📊 Módulos e Funcionalidades

### 1. Motor de Biblioteca Musical (`biblioteca.py`)
* **Inversão Harmônica:** Percorre uma estrutura de dados de "Toques" (Alegre/Triste) e utiliza técnicas de *slicing* para inverter tuplas de frequências, atualizando o dicionário em tempo real.
* **Processamento de Playlists:** Sistema que itera sobre categorias de imagens e emojis, processando caracteres individualmente e invertendo a ordem da lista final de assets.

### 2. Processador de Pixels (`emoji.py`)
* **Matriz de Grade:** Representação de um emoji "Smile" através de uma grade de coordenadas RGB.
* **Algoritmo de Sombreamento:** Identifica pixels de cor amarela `(255, 255, 0)` e aplica uma redução de 50% em cada canal de cor para gerar um efeito de sombra, mantendo os tons pretos inalterados.
* **Visualização:** Renderização automatizada da grade utilizando a função `imshow`.

## 🔧 Como Executar
1. Clone o repositório em sua máquina local.
2. Certifique-se de ter as dependências instaladas:
   ```bash
   pip install matplotlib