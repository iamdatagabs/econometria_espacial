# Econometria Espacial

Repositório de apoio à disciplina de **Econometria Espacial**, com códigos em R, material de análise de dados em painel e um laboratório web interativo.

**Portfólio:** [Gabriel Passos — Engineering Portfolio](https://iamdatagabs.github.io/iamdatagabs/portfolio/) · **Código:** [GitHub](https://github.com/iamdatagabs/econometria_espacial)\n\n## 🌐 Laboratório online

**[Acessar o dashboard — GitHub Pages](https://iamdatagabs.github.io/econometria_espacial/)**

O portal reúne:
- Estatística descritiva e exploração de variáveis;
- Importação de bases próprias em CSV;
- Regressão linear por Mínimos Quadrados Ordinários (MQO), com coeficientes, R² e diagnóstico gráfico de resíduos;
- I de Moran exploratório e diagrama de Moran com matriz K-vizinhos mais próximos;
- Guia conceitual de modelos SLX, SAR, SEM, SDM, SAC e SDEM.

> **Nota metodológica:** o conjunto carregado inicialmente no dashboard é sintético e exclusivamente didático. Importe sua base para explorar os métodos. O painel web não estima modelos SAR/SEM/SDM nem calcula significância do I de Moran; essas etapas exigem os procedimentos reproduzíveis em R.

## Estrutura do repositório

- `PainelEspacial.Rmd`: roteiro de análise de painel espacial em R.
- `codigopainel`: versão textual do material de códigos.
- `guarda.shp`, `guarda.shx`, `guarda.dbf`: arquivos do conjunto geográfico original.
- `index.html`: dashboard estático interativo.
- `.github/workflows/pages.yml`: publicação automática no GitHub Pages.

## Métodos abordados no material em R

- Painel não espacial: pooled, efeitos fixos e aleatórios;
- Testes F/Chow e Hausman;
- Dependência cross-section: CD de Pesaran;
- Matrizes de pesos espaciais: rainha, torre e KNN;
- Modelos espaciais: SAR, SEM, SAC, SDM, SDEM e SLX;
- Estimação por máxima verossimilhança e GMM;
- Critérios de informação e impactos espaciais.

## Como usar o dashboard

1. Abra o [laboratório](https://iamdatagabs.github.io/econometria_espacial/).
2. Carregue um arquivo CSV com cabeçalho na primeira linha.
3. Selecione as variáveis dependente e explicativa.
4. Se a base tiver coordenadas, selecione latitude e longitude para construir a vizinhança KNN por proximidade geográfica.
5. Examine as estatísticas, o ajuste MQO, os resíduos e o I de Moran exploratório.

Para estimar modelos espaciais de painel e realizar testes formais, utilize o roteiro em R e confira os pressupostos e a estrutura da matriz de pesos.

## Tecnologias

R · plm · splm · spdep · spatialreg · HTML · CSS · JavaScript · Chart.js · GitHub Pages.

---

Material acadêmico e didático. Resultados dependem da base utilizada e da especificação econométrica.
