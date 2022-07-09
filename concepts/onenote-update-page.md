---
title: Atualizar o conteúdo da página do OneNote
description: Atualize o conteúdo de uma página do OneNote enviando uma solicitação PATCH para o ponto de extremidade de conteúdo da página. Em seguida, envie um objeto de alteração JSON no corpo da mensagem.
author: jewan-microsoft
ms.localizationpriority: medium
ms.prod: onenote
ms.openlocfilehash: 4ce761de7f1c27ea80db2bd480abf53852368b56
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698062"
---
# <a name="update-onenote-page-content"></a>Atualizar o conteúdo da página do OneNote

**Aplica-se a** Notebooks de consumidores no OneDrive | Notebooks corporativos no Microsoft 365


Para atualizar o conteúdo de uma página do OneNote, envie uma solicitação de PATCH para o ponto de extremidade do *conteúdo* da página:

`PATCH ../notes/pages/{id}/content`</p>

Envie um objeto de alteração JSON no corpo da mensagem. Se a solicitação for bem-sucedida, o Microsoft Graph retornará um código de status de HTTP 204.


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a>Construir a URI de solicitação

Para construir a URI de solicitação, comece com a URL raiz do serviço:

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

Acrescente então o ponto de extremidade do *conteúdo* da página:

- **Obter o HTML da página e todos os valores de *data-id* definidos**<br/><br/>`../pages/{id}/content`   

- **Obter o HTML da página, todos os valores de *data-id* definidos e todos os valores de *id* gerados**<br/><br/>`../pages/{page-id}/content?includeIDs=true` 

A **data-id** e os valores de **id** são usados como identificadores de **destino** para elementos que você deseja atualizar.

 
Sua solicitação de URI completa terá a seguinte aparência:<br/><br/>`https://graph.microsoft.com/v1.0/me/onenote/pages/{id}/content`


Saiba mais sobre a [URL raiz de serviço](/graph/api/resources/onenote-api-overview#root-url).


<a name="message-body"></a>

## <a name="construct-the-message-body"></a>Criar o corpo da mensagem

O HTML de uma página do OneNote contém texto, imagens e outros conteúdos organizados em estruturas como elementos **div**, **img** e **ol**. Para atualizar o conteúdo da página do OneNote, adicione e substitua elementos HTML na página.

Suas alterações serão enviadas no corpo da mensagem como uma matriz de objetos de alteração JSON. Cada objeto especifica o elemento de destino, o novo conteúdo HTML e o que fazer com o conteúdo.

A matriz a seguir define duas alterações. A primeira insere uma imagem acima de um parágrafo como um irmão, e a segunda acrescenta um item em uma lista como um último filho.

> [!NOTE]
> Ao atualizar uma imagem em uma página do OneNote, você não pode usar links www. O serviço não tentará baixar recursos aleatórios. Em vez disso, a imagem deve fazer parte da solicitação, seja por uma url de dados de imagem ou um nome de parte de uma solicitação de várias partes.

```json
[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-data-url-or-part-name" alt="Image above the target paragraph" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the end of the list</li>'
  }
]
```

Veja [mais exemplos](#example-requests).


### <a name="attributes-for-json-change-objects"></a>Atributos de objetos de alteração JSON

Use atributos **target**, **action**, **position** e **content** para definir objetos JSON para solicitações de PATCH.

#### <a name="target"></a>destino

O elemento a ser atualizado. O valor deve ser uma dos seguintes identificadores:

| Identificador | Descrição |  
|------|------|  
| #{data-id} | <p>Essa ID é opcionalmente definida em elementos na HTML de entrada ao [criar uma página](onenote-create-page.md) ou [atualizar uma página](onenote-update-page.md). Coloque um # como prefixo do valor.</p><p> Exemplo:<br/>`'target':'#intro'` tem como destino o elemento `<div data-id="intro" ...>`</p> |  
| id | <p>É a [ID gerada](#generated-ids) do Microsoft Graph e é necessário para a maioria das operações de substituição. Não use # como prefixo.</p><p> Exemplo:<br/>`'target':'div:{33f8a2...}{37}'` tem como destino o elemento `<div id="div:{33f8a2...}{37}" ...>`</p><p>Não confunda esses identificadores com valores de **id** definidos no [HTML de entrada](onenote-input-output-html.md). Todos os valores de **id** enviados no HTML de entrada são descartados.</p> |  
| body | A palavra-chave que tem como destino o primeiro div na página. Não use # como prefixo. |  
| title | A palavra-chave que tem como destino o título da página. Não use # como prefixo. |  
 
#### <a name="action"></a>action

A ação a ser executada no elemento de destino. Veja as [ações com suporte para elementos](#supported-elements-and-actions).

| Ação | Descrição |  
|------|------|  
| append | <p>Adiciona o conteúdo fornecido ao destino como primeiro ou último filho, conforme determinado pelo atributo **position**.</p><p>Aplicável somente a elementos **body**, **div**, **ol** e **ul**.</p> |  
| insert | Adiciona o conteúdo fornecido como irmão antes ou depois do destino, conforme determinado pelo atributo **position**. |  
| prepend | <p>Adiciona o conteúdo fornecido ao destino como um primeiro filho. Atalho para **append** + **before**.</p><p>Aplicável somente a elementos **body**, **div**, **ol** e **ul**.</p> |  
| replace | <p>Substitui o destino pelo conteúdo fornecido.</p><p>A maioria das ações **replace** exige o uso de [ID gerada](#generated-ids) para o destino (exceto os elementos **img** e **object** em um div, que também é compatível com o uso de **data-id**).</p> |  
 
#### <a name="position"></a>position

O local para adicionar o conteúdo fornecido em relação ao elemento de destino. Usa o padrão **after** caso seja omitido.

| Posição | Descrição |  
|------|------|  
| after (padrão) |<p>Com **append**: último filho do elemento de destino.</p><p>Com **insert**: o irmão subsequente do elemento de destino.</p> |
| before | <p>Com **append**: primeiro filho do elemento de destino.</p><p>Com **insert**: o irmão precedente do elemento de destino.</p> |

#### <a name="content"></a>content

Uma cadeia de caracteres em HTML bem formado para adicionar à página e dados binários de imagem ou arquivo. Se o conteúdo contiver dados binários, a solicitação deverá ser enviada usando o tipo de conteúdo `multipart/form-data` com uma parte "Commands" (veja um [exemplo](#multipart-request-with-binary-content).) 
 

<a name="generated-ids"></a>

### <a name="generated-ids"></a>IDs geradas
O Microsoft Graph gera valores de **id** para que os elementos na página possam ser atualizados. Para obter as IDs geradas, use a expressão de cadeia de caracteres de consulta `includeIDs=true` na sua solicitação GET:

`GET ../notes/pages/{page-id}/content?includeIDs=true` 

> [!NOTE]
> A API descarta todos os **valores de ID** definidos no [HTML](onenote-input-output-html.md) de entrada de solicitações de página de criação e de página de atualização.

O exemplo a seguir mostra IDs geradas para um parágrafo e uma imagem no [HTML de saída](onenote-input-output-html.md) de uma página.

```html
<p id="p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}">Some text on the page</p>
<img id="img:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{45}" ... />
```

Os valores de **id** gerados podem ser alterados após uma atualização de página. Então você deve obter valores atuais antes de criar uma solicitação de PATCH que usa esses valores.
 
Você pode especificar elementos de destino usando os valores **data-id** ou **id** seguinte maneira:

- Para as ações **append** e **insert**, você pode usar o ID como o valor de destino.
- Para as ações **replace**, use o ID gerado para todos os elementos, exceto o título da página e imagens e objetos que estejam dentro de um div. 
  - Para substituir um título, use a palavra-chave **título**. 
  - Para substituir imagens e objetos que estejam dentro de um div, use **data-id** ou **id**.

O exemplo a seguir usa o valor **id** para o destino. Não use o prefixo # com um ID gerado.

```json
[
   {
    'target':'p:{33f8a242-7c33-4bb2-90c5-8425a68cc5bf}{40}',
    'action':'insert',
    'position':'before',
    'content':'<p>This paragraph goes above the target paragraph.</p>'
  }
]
```

<a name="support-matrix"></a>

## <a name="supported-elements-and-actions"></a>Elementos e ações compatíveis

Muitos elementos na página podem ser atualizados, mas cada tipo de elemento é compatível com ações específicas. A tabela a seguir mostra os elementos de destino compatíveis com as ações de atualização a que eles dão suporte.

| Elemento | Substituir | Anexar filho | Inserir irmão |  
|------|:------:|:------:|:------:|  
| body<br /> (tem como destino o primeiro div na página) | não | **sim** | não |  
| div<br /> ([absoluto posicionado](onenote-abs-pos.md)) | não | **sim** | não |  
| div<br /> (em um div) | **sim**<br/>(somente id) | **sim** | **sim** |   
| img, object<br /> (em um div) | **sim** | não | **sim** |   
| ol, ul | **sim**<br/>(somente id) | **sim** | **sim** |   
| table | **sim**<br/>(somente id) | não | **sim** |   
| p, li, h1-h6 | **sim**<br/>(somente id) | não | **sim** |   
| title | **sim** | não | não |  
 
<br/>

Os seguintes elementos não dão suporte a nenhuma ação de atualização.

- img ([absoluto posicionado](onenote-abs-pos.md))
- object ([absoluto posicionado](onenote-abs-pos.md))
- tr, td
- meta
- head
- span
- a
- style tags


<a name="examples"></a>

## <a name="example-requests"></a>Solicitações de exemplo

Uma solicitação de atualização contém um ou mais alterações representadas como objetos de alteração JSON. Esses objetos podem definir destinos diferentes na página e outras ações e conteúdos diferentes para os destinos.

Os exemplos a seguir contêm objetos JSON usados em solicitações de PATCH e solicitações de PATCH completo:

- [Acrescentar elementos filho](#append-child-elements)
- [Inserir elementos irmãos](#insert-sibling-elements)
- [Substituir elementos](#replace-elements)
- [Solicitações de PATCH completo](#complete-patch-request-examples)


<a name="append-examples"></a>

### <a name="append-child-elements"></a>Acrescentar elementos filho

A ação **append** adiciona um filho a um elemento **body**, **div** (dentro de um div), **ol** ou **ul**. O atributo **position** determina se deve acrescentar o filho antes ou depois do destino. A posição padrão é **after**.

#### <a name="append-to-a-div"></a>Acrescentar a um div

O exemplo a seguir adiciona dois nós filho ao elemento **div1**. Ele adiciona uma imagem como primeiro filho e um parágrafo como último filho. 

```json
[
 {
    'target':'#div1',
    'action':'append',
    'position':'before',
    'content':'<img data-id="first-child" src="image-url-or-part-name" />'
  },
  {
    'target':'#div1',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph appended to the div</p>'
  }
]
```
 

#### <a name="append-to-the-body-element"></a>Acrescentar ao elemento *body*

Você pode usar o atalho **body** para acrescentar um elemento filho dentro o primeiro div em qualquer página.

O exemplo a seguir adiciona dois parágrafos como primeiro filho e último filho ao primeiro div na página. Não use # com o destino **body**. Este exemplo usa a ação **prepend** como um atalho para **append** + **before**.

```json
[
  {
    'target':'body',
    'action':'prepend',
    'content':'<p data-id="first-child">New paragraph as first child in the first div</p>'
  },
  {
    'target':'body',
    'action':'append',
    'content':'<p data-id="last-child">New paragraph as last child in the first div</p>'
  }
]
```
 

#### <a name="append-to-a-list"></a>Acrescentar a uma lista

O exemplo a seguir adiciona um item de lista como um último filho à lista de destino. A propriedade **list-style-type** é definida porque o item usa um estilo de lista não padrão.

```json
[
  {
    'target':'#circle-ul',
    'action':'append',
    'content':'<li style="list-style-type:circle">Item at the end of the list</li>'
  }
]
```
 

<a name="insert-examples"></a>

### <a name="insert-sibling-elements"></a>Inserir elementos irmãos

A ação **insert** adiciona irmão a um elemento de destino. O atributo **position** determina se deve inserir o irmão antes ou depois do destino. A posição padrão é **after**. Ver [elementos compatíveis com **insert**](#supported-elements-and-actions).

#### <a name="insert-siblings"></a>Inserir irmãos

O exemplo a seguir adiciona dois nós irmãos à página. Adiciona uma imagem acima do elemento **para1** elemento e um parágrafo abaixo do elemento **para2**.

```json
[
  {
     'target':'#para1',
     'action':'insert',
     'position':'before',
     'content':'<img src="image-data-url-or-part-name" alt="Image inserted above the target" />'
  },
  {
    'target':'#para2',
     'action':'insert',
     'content':'<p data-id="next-sibling">Paragraph inserted below the target</p>'
  }
]
```
 

<a name="replace-examples"></a>

### <a name="replace-elements"></a>Substituir elementos

Você pode usar **data-id** ou **id** gerado como o valor de destino para substituir os elementos **img** e **object** que estão em um div. Para substituir um título de página, use a palavra-chave **title**. Para todos os outros [elementos compatíveis com **replace**](#supported-elements-and-actions), você deve usar o ID gerado.

#### <a name="replace-an-image"></a>Substituir uma imagem

O exemplo a seguir substitui uma imagem por um div usando a **data-id** da imagem como destino. 

```json
[
  {
    'target':'#img1',
    'action':'replace',
    'content':'<div data-id="new-div"><p>This div replaces the image</p></div>'
  }
]
```
 

#### <a name="update-a-table"></a>Atualizar um tabela 

Este exemplo mostra como atualizar uma tabela usando seu ID gerado. A substituição dos elementos **tr** e **td** não tem suporte, mas você pode substituir a tabela inteira.

```json
[
  {
    'target':'table:{de3e0977-94e4-4bb0-8fee-0379eaf47486}{11}',
    'action':'replace',
    'content':'<table data-id="football">
      <tr><td><p><b>Brazil</b></p></td><td><p>Germany</p></td></tr>
      <tr><td><p>France</p></td><td><p><b>Italy</b></p></td></tr>
      <tr><td><p>Netherlands</p></td><td><p><b>Spain</b></p></td></tr>
      <tr><td><p>Argentina</p></td><td><p><b>Germany</b></p></td></tr></table>'
  }
]
```
 

#### <a name="change-the-title"></a>Alterar o título 

Este exemplo mostra como alterar o título da página. Para alterar o título, use a palavra-chave **title** como o valor de destino. Não use # com o destino de título.

```json
[
  {
    'target':'title',
    'action':'replace',
    'content':'New title'
  }
]
```
 

#### <a name="update-a-to-do-item"></a>Atualizar um item pendente

O exemplo a seguir usa a ação de substituir para alterar um item de caixa de seleção pendente para um estado concluído.

```json
[
  {
    'target':'#task1',
    'action':'replace',
    'content':'<p data-tag="to-do:completed" data-id="task1">First task</p>'
  }
]
```

Veja [Usar marcas de anotação](onenote-note-tags.md) para saber mais sobre como usar o atributo **data-tag**.


<a name="complete-requests"></a>

### <a name="complete-patch-request-examples"></a>Exemplos de solicitação de PATCH completo

Os exemplos a seguir mostram solicitações de PATCH completo.

#### <a name="request-with-text-content-only"></a>Solicitar apenas com conteúdo de texto

O exemplo a seguir mostra uma solicitação de PATCH que usa o tipo de conteúdo **application/json**. Você pode usar esse formato quando seu conteúdo não contém dados binários.

```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: application/json
Authorization: Bearer {token}

[
   {
    'target':'#para-id',
    'action':'insert',
    'position':'before',
    'content':'<img src="image-data-url" alt="New image from a URL" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]
```
 
<a name="multipart"></a>

#### <a name="multipart-request-with-binary-content"></a>Solicitação de partes múltiplas com conteúdo binário 

O exemplo a seguir mostra uma solicitação de PATCH de diversas partes que inclui dados binários. As solicitações de diversas partes exigem uma parte de "Comandos" que especifica o tipo de conteúdo **application/json** e contém a matriz de objetos de alteração JSON. Outras partes de dados podem conter dados binários. Os nomes de partes são geralmente cadeias de caracteres acrescentadas com a hora atual em milissegundos ou um GUID aleatório.

```http
PATCH https://graph.microsoft.com/v1.0/me/onenote/notebooks/pages/{page-id}/content

Content-Type: multipart/form-data; boundary=PartBoundary123
Authorization: Bearer {token}

--PartBoundary123
Content-Disposition: form-data; name="Commands"
Content-Type: application/json

[
  {
    'target':'img:{2998967e-69b3-413f-a221-c1a3b5cbe0fc}{42}',
    'action':'replace',
    'content':'<img src="name:image-part-name" alt="New binary image" />'
  }, 
  {
    'target':'#list-id',
    'action':'append',
    'content':'<li>Item at the bottom of the list</li>'
  }
]

--PartBoundary123
Content-Disposition: form-data; name="image-part-name"
Content-Type: image/png

... binary image data ...

--PartBoundary123--
```

<a name="request-response-info"></a>

## <a name="request-and-response-information-for-patch-requests"></a>Informações de solicitação e resposta para solicitações de PATCH

| Dados da solicitação | Descrição |  
|------|------|  
| Protocolo | Todas as solicitações usam o protocolo HTTPS de SSL/TLS. |  
| Cabeçalho de autorização | <p>`Bearer {token}`, onde `{token}` é um token de acesso do OAuth 2.0 válido para o aplicativo registrado.</p><p>Se ausente ou inválido, a solicitação falha com um código de status 401. Consulte [Autenticação e permissões](permissions-reference.md).</p> |  
| Cabeçalho content-type | <p>`application/json` para a matriz de objetos de alteração JSON, seja enviado diretamente no corpo da mensagem, seja na parte "Comandos" obrigatória de [solicitações de diversas partes](#multipart-request-with-binary-content).</p><p>As solicitações de diversas partes são necessárias quando se enviam dados binários e usam o tipo de conteúdo `multipart/form-data; boundary=part-boundary`, onde `{part-boundary}` é uma cadeia de caracteres que sinaliza o início e o término de cada parte de dados.</p> |  

<br/> 

| Dados de resposta | Descrição |  
|------|------|  
| Código de êxito | Um código de status de HTTP 204. Nenhum dado JSON é retornado para uma solicitação PATCH. |  
| Erros | Leia [Códigos de erro para APIs do OneNote no Microsoft Graph](onenote-error-codes.md) para saber mais sobre erros do OneNote que poderão ser retornados pelo Microsoft Graph. |  
 
 

<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a>Criar a URL raiz do serviço do Microsoft Graph

A URL raiz do serviço do OneNote usa o formato a seguir para todas as chamadas para o OneNote:

`https://graph.microsoft.com/{version}/me/onenote/`

O segmento `version` na URL representa a versão do Microsoft Graph que você deseja usar. `v1.0` serve para o código de produção estável. `beta` serve para experimentar um recurso que está em desenvolvimento. Os recursos e a funcionalidade na versão beta podem mudar, por isso, você não deve usá-la no código de produção.

`me` serve para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado). `users/{id}` serve para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual. Use a API de [usuários](/graph/v1.0/resources/user.md).

> [!NOTE]
> Você pode obter IDs de usuário fazendo uma solicitação GET em `https://graph.microsoft.com/v1.0/users`.

<a name="permissions"></a>

## <a name="permissions"></a>Permissões

Para atualizar páginas do OneNote, solicite as permissões apropriadas. Escolha o nível mais baixo de permissões que seu aplicativo precisa para realizar o trabalho.

- Notes.ReadWrite
- Notes.ReadWrite.All

Para saber mais sobre escopos de permissão e como eles funcionam, confira [Escopos de permissão do OneNote](permissions-reference.md).
   

<a name="see-also"></a>

## <a name="see-also"></a>Confira também

- [Adicionar imagens e arquivos](onenote-images-files.md)
- [Integrar com o OneNote](integrate-with-onenote.md)
- [Blog de desenvolvedor do OneNote](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Perguntas de desenvolvimento do OneNote no Microsoft Q&A](/answers/topics/microsoft-graph-notes.html)
- [Repositórios do OneNote no GitHub](https://go.microsoft.com/fwlink/?LinkID=390178)
