A finalidade desta unidade é dar uma ideia do que é o Markdown. Para uma análise mais detalhada, consulte os artigos **"Descrição da sintaxe do Markdown"** e **"Especificação do Markdown com um sabor de GitHub"** na seção Resumo no final desse módulo.

## Enfatizar texto
Para usar **itálico** no texto, basta colocar o texto de destino entre asteriscos (`*`) ou sublinhados (`_`).
```markdown
This is *italic* text.
This is also _italic_ text.
```

Crie texto em **negrito** usando dois asteriscos (`**`) ou dois sublinhados (`__`).
```markdown
This is **bold** text.
This is also __bold__ text.
```

Você também pode misturar **tipos de ênfase diferente**s.
```markdown
_This is **italic and bold** text_ using a single underscore for italic and double asterisks for bold.
__This is bold and *italic* text__ using double underscores for bold and single asterisks for italic.
```

Para usar um **asterisco literal**, preceda-o com um caractere de escape, que no GFM é uma barra invertida (`\`).
```markdown
\_This is all \*\*plain\*\* text\_.
```
## Declarar títulos
O HTML fornece títulos de conteúdo, como a tag `<h1>`. Em Markdown, isso tem suporte por meio do símbolo #. Basta usar um # para cada nível de título de 1 a 6.
```markdown
###### This is H6 text
```

## Criar links para imagens e sites
```markdown
![octopus gitHub](images/github.png)
```

![octopus gitHub](images/github.png)

```markdown
[Link to Microsoft Training](https://learn.microsoft.com/pt-br/training)
```
[Link to Microsoft Training](https://learn.microsoft.com/pt-br/training)

## Criar listas
Você pode definir listas ordenadas ou não ordenadas. Você também pode definir itens aninhados por meio de recuos.

- As listas ordenadas começam com números.
- As listas não ordenadas podem usar asteriscos ou traços (`-`).

1. first
2. second
3. Third

- First
	- nested
- Second
- Third

## Criar tabelas
Você pode construir tabelas usando uma combinação de barras verticais (`|`) para quebras de coluna e traços (`-`) para designar a linha anterior como um cabeçalho.

```markdown
First|Second
-|-
1|2
3|4
```

| First | Second |
| ----- | ------ |
| 1     | 2      |
| 3     | 4      |
## Texto da citação
Você pode criar blockquotes usando o caractere maior que (`>`).

```markdown
> This is quoted text.
```
> This is quoted text.
> > Two
> > > Três
> > > > Quatro

## Preencher as lacunas com HTML incorporado
Se você se deparar com uma situação de HTML que não é compatível com o Markdown, você pode usar o HTML incorporado.
```markdown
Here is a<br />line break
```
> Esta é uma  
> quebra de linha

## Trabalhe com código
```javascript
var first = 1;
var second = 2;
var sum = first + second;
```

## Problemas de referência cruzada e solicitações de pull

O GFM é compatível com o uso de uma variedade de formatos de código curto para facilitar a criação de links para problemas e solicitações de pull. A maneira mais fácil de fazer isso é usar o formato `#ID`, como `#3602`
![[links_github.png]]
## Links para commits específicos
Você pode criar um link para um commit colando a respectiva ID ou, simplesmente, usando o respectivo algoritmo de hash seguro (SHA).
![[links_commits.png]]
## Mencionar usuários e equipes
Digitar um símbolo `@` seguido de um nome de usuário do GitHub enviará a essa pessoa uma notificação relativa ao comentário. Isso é chamado de uma "@menção", porque você está mencionando o indivíduo. Você também pode usar `@mention` com equipes dentro de uma organização.
## Monitorar listas de tarefas
Você pode criar listas de tarefas dentro de problemas ou solicitações de pull usando a sintaxe abaixo. Isso pode ser útil para acompanhar o progresso quando usado no corpo de um problema ou solicitação de pull.
```markdown
- [x] First task
- [x] Second task
- [ ] Third task
```
- [x] First task
- [x] Second task
- [ ] Third task
## Comandos de barra "/"
Os comandos de barra "/" podem economizar tempo reduzindo a digitação necessária para criar um Markdown complexo.

Use comandos de barra "/" em qualquer campo de descrição ou de comentário em problemas, solicitações de pull ou discussões em que há suporte para o comando de barra "/".
![[barra_markdown.png]]
