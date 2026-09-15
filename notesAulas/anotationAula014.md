# Resumo Visual: Modos de Exibição no CSS (Display)

Esta tabela sintetiza como o navegador se comporta ao renderizar elementos com diferentes propriedades de `display`.

---

## Tabela Comparativa de Display

| Tipo / Elemento | Ocupa a largura toda? | Quebra linha? | Respeita `width`/`height` e `padding` vertical? |
| :--- | :---: | :---: | :---: |
| **Block-level**<br>`(<div>, <p>, <h1>, <form>)` | **Sim** (100% da largura) | **Sim** (força a próxima linha) | **Sim** (controle total das dimensões) |
| **Inline-level**<br>`(<span>, <a>, <strong>)` | **Não** (apenas o espaço do texto) | **Não** (fica ao lado dos outros) | **Não** (ignora largura/altura e empurrões verticais) |
| **Inline-block**<br>`(<input>, <button>, <img>)` | **Não** (apenas o espaço do texto) | **Não** (fica ao lado dos outros) | **Sim** (o melhor dos dois mundos) |

---

## Explicação Prática do Comportamento

### 1. Block-level (`display: block`)
- Comporta-se como uma **caixa pesada** ou uma linha completa de um caderno.
- Mesmo que o texto seja curto, o elemento ocupa toda a largura horizontal disponível.
- **Ideal para:** Estruturar a página (cabeçalhos, seções, formulários, parágrafos).

### 2. Inline-level (`display: inline`)
- Comporta-se como uma **palavra dentro de uma frase**.
- Ocupa estritamente o tamanho do conteúdo e flui naturalmente com o texto.
- **Limitação:** Não aceita regras de `width`, `height` ou `margin`/`padding` verticais que empurrem outros elementos.
- **Ideal para:** Destacar trechos de texto, links ou tags de estilo inline.

### 3. Inline-block (`display: inline-block`)
- O **híbrido ideal**: comporta-se como `inline` na horizontal (não quebra linha), mas respeita o **Box Model** completo como um `block`.
- Aceita largura, altura, margens e preenchimentos (`padding`) perfeitamente.
- **Ideal para:** Botões, campos de entrada (`<input>`), ícones e cards alinhados em fileira.