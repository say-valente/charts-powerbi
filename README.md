# ComboMatrixChart

Visual customizado para Power BI que combina três visualizações em uma única área: matriz heatmap, gráfico de barras horizontais e gráfico de colunas.

Ideal para análises comparativas com múltiplas dimensões, onde o contexto visual acelera a leitura dos dados.

---

## Funcionalidades

- Matriz heatmap com escala de cor proporcional aos valores
- Gráfico de barras horizontais por linha (totais de linha)
- Gráfico de colunas verticais por coluna (totais de coluna)
- Respeita o formato definido na medida (moeda, percentual, milhares, etc.)
- Ordenação independente por linha e por coluna (padrão, crescente, decrescente)
- Modo percentual: valor original, % do total geral, % da linha, % da coluna
- Suporte a temas do Power BI

---

## Instalação

1. Baixe o arquivo `ComboMatrixChart.pbiviz`
2. No Power BI Desktop, abra o painel **Visualizações**
3. Clique em **"..."** → **Importar um visual de um arquivo**
4. Selecione o arquivo `.pbiviz`

---

## Campos

| Campo | Tipo | Descrição |
|-------|------|-----------|
| **Linhas** | Dimensão | Categoria exibida nas linhas da matriz (ex: cidade, produto) |
| **Colunas** | Dimensão | Categoria exibida nas colunas da matriz (ex: mês, segmento) |
| **Valores** | Medida | Métrica principal (faturamento, quantidade, margem, etc.) |

---

## Configurações

### Layout
- Posição do gráfico de colunas: acima ou abaixo da matriz
- Altura do gráfico de colunas (% da área total)
- Largura do gráfico de barras (% da área total)
- Largura do cabeçalho de linha (% da área total)
- Ordenação de linhas e colunas

### Rótulos
- Modo de exibição: valor original, % do total geral, % da linha, % da coluna
- Exibir/ocultar cada componente (matriz, barras, colunas)
- Fonte e cor dos rótulos

---

## Formatos de medida suportados

O visual lê e aplica automaticamente o formato configurado na medida DAX:

| Formato DAX | Exemplo de saída |
|-------------|-----------------|
| `"R$"\ #,##0.00` | R$ 1.177,90 |
| `#,##0` | 1.177 |
| `#,##0.00` | 1.177,90 |
| `0%` | 85% |
| `0.0%` | 85,3% |
| `$#,##0.00` | $1.177,90 |

Quando nenhum formato está definido, o visual aplica abreviação automática (K / M) com separador pt-BR.

---

## Licença

Copyright (c) 2026 Sayuri Valente Arimori. Todos os direitos reservados.

Este visual é disponibilizado apenas para uso no Power BI.
Não é permitido copiar, modificar, redistribuir, vender ou usar comercialmente sem autorização expressa por escrito.

Para licenciamento comercial, entrar em contato pelo instagram: say.valente

---

*Desenvolvido por Sayuri Valente Arimori*


Copyright (c) 2026 Sayuri Valente Arimori.
Todos os direitos reservados.

Este arquivo é disponibilizado apenas para utilização no Power BI.
Não é permitido copiar, modificar, redistribuir, vender ou usar comercialmente sem autorização expressa por escrito.
