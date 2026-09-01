# Resumo Aula 001

- `<hr>`: Horizontal rule - Cria uma linha horizontal de separação (*sem CSS*).
- `<br>`: Line break - Quebra a linha sem criar outro parágrafo.
- `&lt;` e `&gt;`: Entities (`<` e `>`) - Convertem os símbolos para texto, evitando erros e XSS ao exibir trechos de código (*questão de segurança*). 
- `<pre><code>`: Bloco de código - `<pre>` preserva espaços e quebras de linha; `<code>` aplica a fonte monospaçada de programação.

# Tradução:
- `&lt`: Signfica *Less Than* ou seja menor que `<`
- `&gt`: Signfica  *Greater Than* ou seja maior que `>`
---

## Exemplo Prático

Saiba como printar no Java:

```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello World!!");
    }
}