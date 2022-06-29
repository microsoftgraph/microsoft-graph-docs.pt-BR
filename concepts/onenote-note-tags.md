---
title: Usar marcas de anotação em páginas do OneNote usando a API do OneNote
description: Use o atributo de marca de dados para adicionar e atualizar marcas de anotação internas em uma página do OneNote. Saiba como trabalhar com marcas de anotação em listas e como recuperar marcas de anotação.
author: jewan-microsoft
ms.localizationpriority: medium
ms.prod: onenote
ms.openlocfilehash: 462fd5eeca23118601d32c7050149b131ec48462
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437020"
---
# <a name="use-note-tags-on-onenote-pages"></a>Usar marcas de anotação em páginas do OneNote

**Aplica-se a** notebooks do consumidor no OneDrive | Notebooks empresariais no Microsoft 365

Use o atributo `data-tag` para adicionar e atualizar caixas de seleção, estrelas e outras marcas de anotação incorporadas em uma página do OneNote, conforme mostrado na imagem a seguir.

![Três marcas de anotação exibidas em uma página do OneNote.](images/note-tags-example.png)


<a name="attributes"></a>

## <a name="note-tag-attributes"></a>Atributos de marcas de anotação

No código HTML de uma página do OneNote, uma marca de anotação é representada pelo atributo `data-tag`. Por exemplo:

- Uma caixa de tarefas pendentes desmarcada: `<p data-tag="to-do">`

- Uma caixa de tarefas pendentes marcada: `<p data-tag="to-do:completed">`

- Uma estrela:  `<h2 data-tag="important">`

O valor `data-tag` é composto por uma forma e, às vezes, um status (confira todos os [valores compatíveis](#built-in-note-tags-for-onenote)).

| Propriedade | Descrição |
|:------|:------|
| forma | O identificador da marca de anotação (exemplo: `to-do` ou `important`). |
| status | O status das marcas de anotação da caixa de seleção. Isso só é usado para configurar caixas de seleção como concluídas. |


<a name="note-tags"></a>

## <a name="add-or-update-note-tags"></a>Adicionar ou atualizar marcas de anotação

Para adicionar ou atualizar uma marca de anotação incorporada, basta usar o atributo `data-tag` em um elemento com suporte. Por exemplo, observe um parágrafo marcado como importante:

```html
<p data-tag="important">...</p>
```

Separe várias marca de anotação por vírgulas:

```html
<p data-tag="important, critical">...</p>
```

Você pode definir uma `data-tag` nos seguintes elementos:

- p
- ul, ol, li (saiba mais sobre [marcas de anotação em listas](#note-tags-on-lists))
- img
- h1 – h6
- título

Confira [Marcas de anotação incorporadas](#built-in-note-tags-for-onenote) para obter uma lista de marcas de anotação que podem ser usadas com o Microsoft Graph. Não há suporte para adicionar ou atualizar marcas personalizadas usando o Microsoft Graph.

### <a name="examples"></a>Exemplos

Veja uma lista simples de tarefas pendentes com o primeiro item marcado como concluído.

```html
<p data-tag="to-do:completed" data-id="prep">Till garden bed</p>
<p data-tag="to-do" data-id="spring">Plant peas and spinach</p>
<p data-tag="to-do" data-id="summer">Plant tomatoes and peppers</p>
```

Observe que as `<p>` marcas acima incluem cada uma o atributo `data-id`. Isso facilita a atualização das marcas de anotação da caixa de seleção. Por exemplo, a seguinte solicitação marca o item “plantio da primavera” como concluído.

```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#spring',
    'action':'replace',
    'content':'<p data-tag="to-do:completed"  data-id="spring">Plant peas and spinach</p>'
  }
]
```

A seguinte solicitação cria uma página que contém todas as [marcas de anotação incorporadas](#built-in-note-tags-for-onenote).

```html
POST https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages

Content-Type: text/html
Authorization: Bearer {token}


<!DOCTYPE html>
<html>
  <head>
    <title data-tag="to-do:completed">All built-in note tags</title>
  </head>
  <body>
    <h1 data-tag="important">Paragraphs with built-in note tags</h1>
    <p data-tag="to-do">to-do</p>
    <p data-tag="important">important</p>
    <p data-tag="question">question</p>
    <p data-tag="definition">definition</p>
    <p data-tag="highlight">highlight</p>
    <p data-tag="contact">contact</p>
    <p data-tag="address">address</p>
    <p data-tag="phone-number">phone-number</p>
    <p data-tag="web-site-to-visit">web-site-to-visit</p>
    <p data-tag="idea">idea</p>
    <p data-tag="password">password</p>
    <p data-tag="critical">critical</p>
    <p data-tag="project-a">project-a</p>
    <p data-tag="project-b">project-b</p>
    <p data-tag="remember-for-later">remember-for-later</p>
    <p data-tag="movie-to-see">movie-to-see</p>
    <p data-tag="book-to-read">book-to-read</p>
    <p data-tag="music-to-listen-to">music-to-listen-to</p>
    <p data-tag="source-for-article">source-for-article</p>
    <p data-tag="remember-for-blog">remember-for-blog</p>
    <p data-tag="discuss-with-person-a">discuss-with-person-a</p>
    <p data-tag="discuss-with-person-b">discuss-with-person-b</p>
    <p data-tag="discuss-with-manager">discuss-with-manager</p>
    <p data-tag="send-in-email">send-in-email</p>
    <p data-tag="schedule-meeting">schedule-meeting</p>
    <p data-tag="call-back">call-back</p>
    <p data-tag="to-do-priority-1">to-do-priority-1</p>
    <p data-tag="to-do-priority-2">to-do-priority-2</p>
    <p data-tag="client-request">client-request</p>
    <h1 data-tag="important">Paragraphs with check boxes marked with "completed" status</h1>
    <p data-tag="to-do:completed">to-do:completed</p>
    <p data-tag="discuss-with-person-a:completed">discuss-with-person-a:completed</p>
    <p data-tag="discuss-with-person-b:completed">discuss-with-person-b:completed</p>
    <p data-tag="discuss-with-manager:completed">discuss-with-manager:completed</p>
    <p data-tag="schedule-meeting:completed">schedule-meeting:completed</p>
    <p data-tag="call-back:completed">call-back:completed</p>
    <p data-tag="to-do-priority-1:completed">to-do-priority-1:completed</p>
    <p data-tag="to-do-priority-2:completed">to-do-priority-2:completed</p>
    <p data-tag="client-request:completed">client-request:completed</p>
    <h1 data-tag="important">Multiple note tags</h1>
    <p data-tag="project-a,  client-request:completed">Two note tags:  project-a, client-request:completed</p>
    <p data-tag="idea, send-in-email, question">Three note tags:  idea, send-in-email, question</p>
    <h1 data-tag="important">Using note tags with other elements</h1>
    <p><b>Note tag on a list item:</b></p>
    <ul>
      <li data-tag="to-do-priority-1:completed">Make a to-do list</li>
    </ul>
    <p><b>Note tag on an image:</b></p>
    <img data-tag="source-for-article" src="https://placecorgi.com/200" />
    <p><b>Note tag with embedded style:</b></p>
    <p data-tag="important">Next time, <b>don't</b> forget to invite <span style="background-color:yellow">Dan</span>.</p>
  </body>
</html>
```

Para obter mais informações sobre a criação de páginas, confira [Criar páginas do OneNote](onenote-create-page.md). Para obter mais informações sobre a atualização de páginas, confira [Atualizar páginas do OneNote](onenote-update-page.md).


<a name="note-tags-lists"></a>

## <a name="note-tags-on-lists"></a>Marcas de anotação em listas

Veja algumas orientações para trabalhar com marcas de anotação em listas:

- Use os elementos `p` para listas de tarefas pendentes. Eles não exibem um marcador ou número e são mais fáceis de atualizar.

- Para criar ou atualizar listas que exibem a **mesma** marca de anotação para todos os itens da lista, defina `data-tag` no `ul` ou no `ol`. Para atualizar a lista inteira, será necessário redefinir `data-tag` no `ul` ou no `ol`.

- Para criar ou atualizar listas que exibem uma marca de anotação **exclusiva** para alguns ou todos os itens da lista, defina `data-tag` nos elementos `li` e não aninhe os elementos `li` em um `ul` ou no `ol`. Para atualizar a lista inteira, será preciso remover o `ul`, que é retornado na saída HTML, e fornecer somente os elementos `li` não aninhados

- Para atualizar elementos `li` específicos, defina individualmente como destino os elementos `li` e defina a `data-tag` no elemento `li`. Qualquer elemento `li` tratado individualmente pode ser atualizado para exibir uma marca de anotação exclusiva, independentemente de como a lista foi originalmente definida.

  As diretrizes são baseadas nas seguintes regras aplicadas pelo Microsoft Graph:

  - A configuração `data-tag` para um `ul` ou `ol` substitui todas as configurações em elementos filho `li`. Isso se aplica mesmo quando o `ul` ou `ol` não especifica um `data-tag`, mas seus elementos filho `li` sim.

    Por exemplo, se você criar um `ul` ou `ol` que defina `data-tag="project-a"`, todos os seus itens de lista serão exibidos na marca de anotação *Project A*. Ou, se `ul` ou `ol` não definir um `data-tag`, nenhum dos seus itens exibirá uma marca de anotação. Essa substituição acontece independentemente das configurações explícitas nos elementos filho `li`.

- As configurações exclusivas `data-tag` são liquidadas para itens de lista nas seguintes condições:

  - Os elementos `li` não estão aninhados em um `ul` ou `ol` em uma solicitação de criação ou atualização.

  - Um elemento `li` é tratado individualmente em uma solicitação de atualização.

- Os elementos `li` não aninhados enviados no HTML de entrada são retornados em um `ul` no HTML de saída.

- No HTML de saída, todas as configurações da lista `data-tag` são definidas em elementos `span` nos itens da lista.


O código a seguir mostra como algumas dessas regras são aplicadas. O HTML de entrada cria duas listas com marcas de anotação. O HTML de saída é o que é retornado para as listas quando você recupera o conteúdo da página.

#### <a name="input-html"></a>HTML de entrada

```html
<!--To display the same note tag on all list items, define note tags on the ul or ol.-->
<ul data-tag="project-a" data-id="agenda">
  <li>An item with a Project A note tag</li>
  <li>An item with a Project A note tag</li>
</ul>

<!--To display unique note tags on list items, don't nest li elements in a ul or ol.-->
<li data-tag="idea" data-id="my-idea">An item with an Idea note tag</li>
<li data-tag="question" data-id="my-question">An item with a Question note tag</li>
```

#### <a name="output-html"></a>HTML de saída

```html
<ul>
  <li><span data-tag="project-a">An item with a Project A note tag</span></li>
  <li><span data-tag="project-a">An item with a Project A note tag</span></li>
</ul>
<br />
<ul>
  <li style="..."><span data-tag="idea">An item with an Idea note tag</span></li>
  <li style="..."><span data-tag="question">An item with a Question note tag</span></li>
</ul>
```

<a name="output-html"></a>

## <a name="retrieve-note-tags"></a>Recuperar marcas de anotação

As marcas de anotação incorporadas são incluídas no HTML de saída quando você obtém o conteúdo da página:

`GET ../api/v1.0/pages/{page-id}/content`

Um atributo `data-tag` no HTML de saída sempre inclui um valor de forma e inclui apenas um status se ele representar uma marca de anotação de caixa de seleção definida como concluída. Os exemplos a seguir mostram o HTML de entrada usado para criar algumas marcas de anotação e o HTML de saída que é retornado.

#### <a name="input-html"></a>HTML de entrada

```html
<h1>Status meeting</h1>
<p data-tag="important">Next week's meeting has been moved to <b>Wednesday</b>.</p>
<p data-tag="question">What are the exact dates for the conference?</p>
<p>Upcoming training opportunities. See Katie for more info.</p>
<p data-tag="project-a">Around the room updates.</p>
<ul data-tag="critical">
  <li>Design handouts</li>
  <li>Plan keynote</li>
</ul>
```

#### <a name="output-html"></a>HTML de saída

```html
<h1 style="...">Status meeting</h1>
<p data-tag="important">Next week's meeting has been moved to <span style="font-weight:bold">Wednesday</span>.</p>
<p data-tag="question">What are the exact dates for the conference?</p>
<p>Upcoming training opportunities. See Katie for more info.</p>
<p data-tag="project-a">Around the room updates.</p>
<ul>
  <li><span data-tag="critical">Design handouts</span></li>
  <li><span data-tag="critical">Plan keynote</span></li>
</ul>
```

Observe que o atributo `data-tag` definido no nível de lista é enviado para seus itens de lista. Para obter mais informações sobre como usar marcas de anotação com listas, confira [Marcas de anotação em listas](#note-tags-on-lists).

> [!NOTE]
> No HTML de saída, a definição e as marcas de anotação remember-for-later são retornadas como `data-tag="remember-for-later"`. O elemento `title` não retorna informações sobre marcas de anotação.




<a name="built-in-tags"></a>

## <a name="built-in-note-tags-for-onenote"></a>Marcas de anotação incorporadas para o OneNote

O OneNote inclui as seguintes marcas de anotação incorporadas:

![Todas as marcas de anotação internas.](images/note-tags-all.png)

Os valores que você pode atribuir ao atributo `data-tag` são mostrados na lista a seguir. As marcas personalizadas não são suportadas.

- `shape[:status]`
- `to-do`
- `to-do:completed`
- `important`
- `question`
- `definition`
- `highlight`
- `contact`
- `address`
- `phone-number`
- `web-site-to-visit`
- `idea`
- `password`
- `critical`
- `project-a`
- `project-b`
- `remember-for-later`
- `movie-to-see`
- `book-to-read`
- `music-to-listen-to`
- `source-for-article`
- `remember-for-blog`
- `discuss-with-person-a`
- `discuss-with-person-a:completed`
- `discuss-with-person-b`
- `discuss-with-person-b:completed`
- `discuss-with-manager`
- `discuss-with-manager:completed`
- `send-in-email`
- `schedule-meeting`
- `schedule-meeting:completed`
- `call-back`
- `call-back:completed`
- `to-do-priority-1`
- `to-do-priority-1:completed`
- `to-do-priority-2`
- `to-do-priority-2:completed`
- `client-request`
- `client-request:completed`


<a name="request-response-info"></a>

## <a name="response-information"></a>Informações de resposta

O Microsoft Graph retornará as seguintes informações na resposta.

| Dados de resposta | Descrição |
|------|------|
| Código de êxito | Um código de status HTTP 201 para uma solicitação POST bem-sucedida e um código de status HTTP 204 para uma solicitação PATCH bem-sucedida. |
| Erros | Leia [Códigos de erro para APIs do OneNote no Microsoft Graph](onenote-error-codes.md) para saber mais sobre erros do OneNote que poderão ser retornados pelo Microsoft Graph. |


<a name="permissions"></a>

## <a name="permissions"></a>Permissões

Para criar ou atualizar páginas do OneNote, solicite permissões apropriadas. Escolha o nível mais baixo de permissões que seu aplicativo precisa para realizar o trabalho.

#### <a name="permissions-for-post-pages"></a>Permissões para páginas POST

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All

#### <a name="permissions-for-patch-pages"></a>Permissões para páginas PATCH

- Notes.ReadWrite
- Notes.ReadWrite.All

Para saber mais sobre escopos de permissão e como eles funcionam, confira [Escopos de permissão do OneNote](permissions-reference.md).


<a name="see-also"></a>

## <a name="see-also"></a>Confira também

- [Criar páginas do OneNote](onenote-create-page.md)
- [Atualizar o conteúdo da página do OneNote](onenote-update-page.md)
- [Integrar com o OneNote](integrate-with-onenote.md)
- [Blog de desenvolvedor do OneNote](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Perguntas de desenvolvimento do OneNote no Microsoft Q&A](/answers/topics/microsoft-graph-notes.html)
- [Repositórios do OneNote no GitHub](https://go.microsoft.com/fwlink/?LinkID=390178)
