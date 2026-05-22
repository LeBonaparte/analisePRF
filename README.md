# Análise de Acidentes em Rodovias Federais e Efetividade dos Radares

### Posicionamento Estratégico de Radares nas Rodovias Federais Brasileiras

Análise exploratória de dados com 17.502 registros de acidentes em rodovias federais e 1.048 radares ativos, cruzando dados da PRF e da ANTT para identificar zonas críticas, avaliar o impacto dos radares e sugerir realocações estratégicas.

🔗 🔗 **[Acesse o relatório completo](https://lebonaparte.github.io/analisePRF/relatorio_gestao_rodovias.html)**

---

## Sobre o Projeto

Este projeto faz parte da minha jornada de aprendizado em análise de dados. O objetivo foi aplicar técnicas de limpeza, pré-processamento, análise exploratória e geoespacial em dados reais da segurança pública viária, gerando recomendações concretas para gestores de infraestrutura.

O relatório final foi desenvolvido em HTML com identidade visual própria, gráficos embutidos, mapas interativos e navegação por seções — tudo em um único arquivo autocontido.

---

## Principais Achados

- **BR-101 e BR-116 concentram ~33% de todos os acidentes** e lideram o ranking de mortes no trimestre
- **Radares funcionam:** acidentes próximos a radares (≤10km) têm **47% menos fatalidade** do que os distantes
- **678 acidentes fatais** ocorreram a mais de 50km de qualquer radar — lacuna crítica de cobertura
- **Nordeste é a região mais vulnerável:** BA, PE, MA, PB, PI e AL concentram a maioria das zonas críticas sem cobertura
- **173 radares candidatos à realocação** identificados com 0 mortes e menos de 5 acidentes no raio de 10km
- **Madrugada é o período mais letal:** 4h da manhã registra 16% de fatalidade — 5× mais que 9h

---

## Estrutura do Repositório

```
analise-acidentes-rodovias/
│
├── relatorio_gestao_rodovias.html   # Relatório completo com gráficos e mapas embutidos
├── README.md                        # Este arquivo
├── notebooks/
│   └── analise_rodovias.ipynb       # Notebook com toda a análise
├── outputs/
│   ├── graficos/                    # PNGs dos gráficos gerados
│   └── mapas/                       # HTMLs dos mapas interativos (Folium)
├── apresentacao/
│   └── analise_rodovias_radares.pptx
└── data/
    └── README.md                    # Instruções para baixar os dados brutos
```

---

## Ferramentas Utilizadas

| Ferramenta | Uso |
|---|---|
| Python | Linguagem principal |
| Pandas | Manipulação e limpeza de dados |
| Matplotlib | Visualizações estáticas |
| Seaborn | Heatmaps e estilo visual |
| Folium | Mapas interativos geoespaciais |
| Scipy (cKDTree) | Cálculo de distâncias geoespaciais |
| Scikit-learn (KMeans) | Agrupamento geográfico de zonas críticas |
| Jupyter Notebook | Ambiente de desenvolvimento |
| VS Code | Editor de código |
| HTML / CSS | Relatório final |

---

## Fonte dos Dados

- **PRF — Polícia Rodoviária Federal:** [Dados Abertos de Acidentes](https://www.gov.br/prf/pt-br/acesso-a-informacao/dados-abertos/dados-abertos-da-prf)
  - Arquivo: `datatran2026.csv` — 17.502 registros, 30 variáveis
- **ANTT — Agência Nacional de Transportes Terrestres:** [Portal de Dados Abertos — Radares](https://dados.antt.gov.br/dataset/radar)
  - Arquivo: `dados-dos-radares2_2026.csv` — 1.048 radares, 15 variáveis
- **Período analisado:** Janeiro a Março de 2026

> ⚠️ Os arquivos CSV brutos não estão incluídos no repositório por excederem o limite de tamanho do GitHub. Baixe diretamente nas fontes acima e coloque na pasta `data/`.

---

## Sobre

Desenvolvido por **Leticia Guedea Bonaparte**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/leticia-guedea-bonaparte/)
