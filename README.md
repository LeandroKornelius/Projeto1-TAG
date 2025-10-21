# 🧠 Projeto 1 – Teoria e Aplicação de Grafos (TAG) – UnB 2025/2
Autor: Leandro Beloti Kornelius

---

## 📘 Descrição do Projeto

Este projeto tem como objetivo **analisar uma rede social real** por meio de conceitos e métricas de **Teoria dos Grafos**, utilizando o conjunto de dados público **Facebook Social Network** disponibilizado pelo repositório [SNAP Stanford](https://snap.stanford.edu/data/egonets-Facebook.html).

A análise envolve:
- **Construção de um grafo** representando usuários e suas conexões;  
- **Extração de uma amostra** de 2.000 nós e suas respectivas arestas;  
- **Cálculo de métricas de centralidade** (grau, intermediação, proximidade e autovetor);  
- **Detecção de comunidades** pelo algoritmo de **Louvain**;  
- **Visualização das comunidades e dos nós mais influentes**;  
- **Discussão interpretativa** sobre influência, importância e propagação de informação na rede.

---

## 💡 Etapas de Implementação

1. **Coleta e Amostragem de Dados**  
   - Carregamento do dataset original (`facebook_combined.txt`).  
   - Seleção aleatória de 2.000 nós e criação do subgrafo induzido.

2. **Construção do Grafo**  
   - Leitura e criação do grafo usando `NetworkX`.  
   - Verificação de conectividade e identificação da componente gigante.

3. **Detecção de Comunidades**  
   - Aplicação do algoritmo de **Louvain** para particionar a rede.  
   - Cálculo da **modularidade** e armazenamento das comunidades como atributos.

4. **Cálculo de Métricas de Centralidade**  
   - Grau, Intermediação (Betweenness), Proximidade (Closeness) e Autovetor (Eigenvector).  
   - Identificação dos nós mais influentes segundo cada métrica.

5. **Visualização e Interpretação**  
   - Plotagem dos grafos coloridos por comunidade e dos nós centrais destacados.  
   - Exportação de resultados e visualizações para Gephi (opcional).  
   - Interpretação dos resultados e discussão sobre influência e propagação de informação.