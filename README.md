# Cartas de Controle X̄ e R — Tópico 6.2
## Cartas de Shewhart para Variáveis: Média e Amplitude

**Autor:** Andre Luiz Marques Serrano  
**Disciplina:** Controle Estatístico da Qualidade  
**Referência:** Montgomery, D. C. (2016). *Introdução ao Controle Estatístico da Qualidade*. 7ª ed. LTC. Seção 6.2, pp. 238–274.

---

## Descrição

Este projeto implementa as **Cartas de Controle X̄ (média) e R (amplitude)** conforme o Tópico 6.2 do livro *Introdução ao Controle Estatístico da Qualidade* de Douglas C. Montgomery (7ª ed., 2016).

As cartas de Shewhart para variáveis são as ferramentas mais utilizadas no Controle Estatístico do Processo (CEP) quando a característica de qualidade é mensurável em escala contínua. O par X̄-R monitora simultaneamente a **localização** (média) e a **dispersão** (variabilidade) do processo.

---

## Conteúdo do Projeto

| Arquivo | Descrição |
|---------|-----------|
| `notebook_*.ipynb` | Notebook Jupyter com código, gráficos e interpretações |
| `README.md` | Este arquivo — documentação do projeto |

---

## Tópicos Abordados

- Construção das Cartas X̄ e R (Fase I — estimação dos limites)
- Constantes d₂, D₃, D₄, A₂ para diferentes tamanhos de amostra
- Análise de padrões: regras de Western Electric (WE)
- Revisão dos limites com exclusão de pontos fora de controle
- Capacidade do processo: Cp, Cpk, Cpm
- Análise de variações: variações de Fase I e Fase II
- Exercício resolvido: Exemplo 6.1 — Diâmetros de anéis de pistão (Tabela 6.1)

---

## Exercício Resolvido

> **Exemplo 6.1 — Diâmetros internos de anéis de pistão (n=5, m=25, Tabela 6.1, p. 242)**

O notebook reproduz integralmente o exemplo do livro, com cálculo passo a passo de todos os parâmetros, comparação com os valores tabelados por Montgomery e interpretação estatística detalhada de cada gráfico.

---

## Bibliotecas Utilizadas

| Biblioteca | Finalidade |
|------------|------------|
| `numpy` | Cálculo vetorial de médias, amplitudes e constantes de controle |
| `pandas` | Estruturação dos dados amostrais e tabelas de resultados |
| `matplotlib` | Construção das cartas de controle com anotações e zonas |
| `scipy.stats` | Distribuições estatísticas e testes de normalidade |
| `warnings` | Supressão de avisos não críticos durante execução |

**Instalação:**

```bash
pip install numpy pandas matplotlib scipy
```

---

## Gráficos Gerados

Os gráficos são gerados automaticamente ao executar o notebook. Todos utilizam paleta de cores neutras (escala de cinzas) adequada para publicações acadêmicas.

| Arquivo | Descrição |
|---------|-----------|
| `fig01_cartas_xbar_R.png` | Cartas X̄ e R — Fase I com limites calculados |
| `fig02_cartas_xbar_R_revisadas.png` | Cartas X̄ e R — Fase I revisada (pontos excluídos) |
| `fig03_zonas_WE.png` | Cartas X̄ com zonas de Western Electric |
| `fig04_capacidade.png` | Histograma com especificações e índices Cp/Cpk |
| `fig05_normalidade.png` | Gráfico de probabilidade normal e histograma |

---

## Como Executar

### Google Colab (recomendado)

1. Acesse [colab.research.google.com](https://colab.research.google.com)
2. Clique em **Arquivo → Fazer upload de notebook**
3. Selecione o arquivo `.ipynb` deste projeto
4. Execute todas as células com **Runtime → Run all**

### Localmente (Jupyter)

```bash
# Instalar dependências
pip install numpy pandas matplotlib scipy jupyter

# Iniciar o Jupyter
jupyter notebook notebook_*.ipynb
```

---

## Referência Bibliográfica

Montgomery, D. C. (2016). *Introdução ao Controle Estatístico da Qualidade*. 7ª ed. Rio de Janeiro: LTC.

---

*Andre Luiz Marques Serrano*
