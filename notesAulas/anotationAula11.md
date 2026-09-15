#  Guia Prático: Seletores e Especificidade no CSS

## 1. As 3 Formas de Selecionar Elementos

| Seletor | Sintaxe CSS | Uso no HTML | Quando Usar |
| :--- | :--- | :--- | :--- |
| **Tag** | `h1 { ... }` | `<h1>Texto</h1>` | Estilos genéricos para **todos** os elementos daquela tag. |
| **Classe** | `.minha-classe { ... }` | `<h2 class="minha-classe">` | Estilos **reutilizáveis** em vários elementos diferentes. |
| **ID** | `#meu-id { ... }` | `<h1 id="meu-id">` | Estilo único para um **único elemento** específico da página. |

---

## 2. A Hierarquia de Poder (Especificidade)

O CSS decide qual estilo aplicar com base na prioridade do seletor. **O mais forte sempre sobrescreve os mais fracos**, independentemente da ordem no arquivo CSS.

$$\text{ID (\#)} > \text{Classe (.)} > \text{Tag (h1, p, h2)}$$

### Exemplo Prático:

```html
<!-- HTML -->
<h1 id="titulo-principal" class="titulo-destaque">
  Exemplo de Especificidade
</h1>