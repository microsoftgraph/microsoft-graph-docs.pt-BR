---
title: Criar páginas do OneNote
description: " Blocos de anotações empresariais no Microsoft 365"
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
ms.openlocfilehash: 815c42257449dde122958cc4ab3f9293387c0cb3
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472787"
---
# <a name="create-onenote-pages"></a>Criar páginas do OneNote

**Aplica-se a**: Blocos de anotações de consumidor no OneDrive | Blocos de anotações empresariais no Microsoft 365

Para criar uma página do OneNote, você envia uma solicitação POST para um ponto de extremidade de *pages*. Por exemplo:

`POST ../notes/sections/{id}/pages`

<br/>

Envie o HTML que define a página no corpo da mensagem. Se a solicitação for bem-sucedida, o Microsoft Graph retornará um código de status de HTTP 201.


> **Observação:** para saber mais sobre as solicitações POST que você pode enviar para criar seções, grupos de seções e blocos de anotações, consulte a nossa [referência interativa do REST](https://dev.onenote.com/docs).


<a name="request-uri"></a>

## <a name="construct-the-request-uri"></a>Construir a URI de solicitação

Para construir a URI de solicitação POST, comece com a URL raiz do serviço:

`https://graph.microsoft.com/v1.0/me/onenote`

<br/>

Depois acrescente o ponto de extremidade de *pages*:

- **Criar uma página em qualquer seção (especificada pelo nome da seção)**<br/><br/>`.../pages?sectionName=DefaultSection`

- **Criar uma página em qualquer seção (especificada pela ID)**<br/><br/>`.../sections/{section-id}/pages` 

Se você estiver criando páginas no bloco de anotações pessoal do usuário, o Microsoft Graph também fornecerá pontos de extremidade que você pode usar para criar páginas no bloco de anotações padrão:

- **Criar uma página na seção padrão do bloco de anotações padrão**<br/><br/>`../pages` 



Sua URI de solicitação completa parecerá com um dos seguintes exemplos:

- `https://graph.microsoft.com/v1.0/me/onenote/sections/{id}/pages`
- `https://graph.microsoft.com/v1.0/me/onenote/pages?sectionName=Homework`

Saiba mais sobre a [URL raiz de serviço](/graph/api/resources/onenote-api-overview?view=graph-rest-1.0#root-url).

<a name="post-pages-section-name"></a>

### <a name="using-the-sectionname-url-parameter"></a>Usar o parâmetro de URL *sectionName*

As seguintes regras aplicam-se ao usar o parâmetro *sectionName* para a criação de uma página em uma seção nomeada no bloco de anotações padrão:

- Apenas seções de nível superior podem ser referenciadas (não as seções nos grupos de seções).

- Se não houver uma seção com o nome especificado no bloco de anotações padrão, a API a criará. Os seguintes caracteres não são permitidos nos nomes de seção: `? * \ / : < > | & # " % ~`

- Os nomes das seções não diferenciam letras maiúsculas de minúsculas para correspondência, mas a diferença entre maiúsculas e minúsculas é preservada ao criar seções. Portanto, "Minha Nova Seção" será exibida assim, mas também seria feita a correspondência de "minha nova seção" nas postagens subsequentes.

- Os nomes das seções devem ser codificados por URL. Por exemplo, os espaços devem ser codificados como *20%*.

- O parâmetro *sectionName* só é válido com a rota `../notes/pages` (não com `../notes/sections/{id}/pages`).

Como serão criadas seções caso não existam, é seguro usar essa chamada com todas as páginas que o seu aplicativo criar. Os usuários podem renomear as seções, mas a API criará uma nova seção com o nome da seção que você fornecer. 

> **Observação:** os links retornados pela API para as páginas de uma seção renomeada ainda abrirão essas páginas antigas. 


<a name="message-body"></a>

## <a name="construct-the-message-body"></a>Criar o corpo da mensagem

O HTML que define o conteúdo da página se chama *HTML de entrada*. O HTML de entrada é compatível com um [subconjunto de HTML e CSS padrão](#supported-html-and-css-for-onenote-pages), com a adição de atributos personalizados. (Os atributos personalizados, como **data-id** e **data-render-src**, são descritos em [HTML de entrada e de saída](onenote-input-output-html.md).) 

Envie o HTML de entrada no corpo da mensagem da solicitação POST. Você pode enviar o HTML de entrada diretamente no corpo da mensagem usando o tipo de conteúdo `application/xhtml+xml` ou `text/html`, ou pode enviá-lo na parte "Apresentação" de uma solicitação de diversas partes. 

O exemplo a seguir envia o HTML de entrada diretamente no corpo da mensagem.

```html
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: application/xhtml+xml

<!DOCTYPE html>
<html>
  <head>
    <title>A page with a block of HTML</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>This page contains some <i>formatted</i> <b>text</b> and an image.</p>
    <img src="https://..." alt="an image on the page" width="500" />
  </body>
</html>
```

<br/>

Se você estiver enviando dados binários, use uma [solicitação de diversas partes](#example-request). 

> **Observação:** para simplificar a programação e a consistência em seu aplicativo, use as solicitações de diversas partes para criar todas as páginas. É uma boa ideia usar uma biblioteca para criar mensagens de diversas partes. Isso reduz o risco da criação de cargas mal formadas.


<a name="input-html-rules"></a>

### <a name="requirements-and-limitations-for-input-html-in-post-pages-requests"></a>Requisitos e limitações para HTML de entrada em solicitações de páginas POST

Ao enviar HTML de entrada, lembre-se desses requisitos e limitações gerais:  

- O HTML de entrada deve ser codificado em UTF-8 e Extensible HTML bem elaborado. Todas as marcas de início do contêiner exigem marcas de fechamento correspondentes. Todos os valores do atributo devem estar entre aspas simples ou duplas.  <!--docs say MUST be encoded-->

- O código JavaScript, os arquivos inclusos e CSS são removidos. 

- Os formulários HTML são removidos totalmente.  

- O Microsoft Graph é compatível com um [subconjunto de elementos HTML](#supported-html-and-css-for-onenote-pages). 

- O Microsoft Graph é compatível com um subconjunto de atributos HTML comuns e um conjunto de atributos personalizados, como o atributo **data-id** usado para atualizar as páginas. Confira os atributos compatíveis em [HTML de entrada e de saída](onenote-input-output-html.md).


<a name="supported-html"></a>

### <a name="supported-html-and-css-for-onenote-pages"></a>HTML e CSS compatíveis com páginas do OneNote

Nem todos os elementos, atributos e propriedades são compatíveis (em HTML4, Extensible HTML, CSS, HTML5 etc.). Em vez disso, o Microsoft Graph aceita um conjunto limitado de HTML mais adequado à forma como as pessoas usam o OneNote. Saiba mais em [Suporte de marca HTML para páginas](https://dev.onenote.com/docs#/introduction/html-tag-support-for-pages). Se uma marca não estiver listada aqui, provavelmente será ignorada.

<!--Microsoft Graph only accepts UTF-8 data. Be sure that all requests are encoded that way, and your content-type headers indicate that as well. xx our examples don't show this-->

A lista a seguir mostra os tipos de elementos básicos compatíveis com o Microsoft Graph:

- `<head>` e `<body>`</p>
- `<title>` e `<meta>` que definem a data de criação e o título de página</p>
- `<h1>` a `<h6>` para títulos de seção</p>
- `<p>` para parágrafos</p>
- `<ul>`, `<ol>` e `<li>` para listas e itens de lista</p>
- `<table>`, `<tr>` e `<td>`, incluindo tabelas aninhadas</p>
- `<pre>` para texto pré-formatado (preserva as quebras de linha e espaços em branco)</p>
- `<b>` e `<i>` para estilos de caractere em negrito e itálico</p>

O Microsoft Graph preserva o conteúdo semântico e a estrutura básica do HTML de entrada ao criar páginas, mas converte o HTML de entrada para usar o conjunto compatível de HTML e CSS. Os recursos que não existem no OneNote não têm nada para ser convertido, portanto, podem não ser reconhecidos no HTML de origem. 


<a name="example"></a>

## <a name="example-request"></a>Exemplo de solicitação

Esse exemplo de solicitação de diversas partes cria uma página que contém imagens e um arquivo inserido. A parte **Apresentação** necessária contém o HTML de entrada que define a página. A parte **imageBlock1** contém os dados de imagem binária, e **fileBlock1** contém os dados do arquivo binário. As partes de dados também podem conter HTML e, nesse caso, o Microsoft Graph [processa o HTML como uma imagem](onenote-images-files.md#add-an-image-using-binary-data) na página do OneNote. 

```html
POST https://graph.microsoft.com/v1.0/me/onenote/pages
Authorization: Bearer {token}
Content-Type: multipart/form-data; boundary=MyPartBoundary198374

--MyPartBoundary198374
Content-Disposition:form-data; name="Presentation"
Content-Type:text/html

<!DOCTYPE html>
<html>
  <head>
    <title>A page with rendered images and an attached file</title>
    <meta name="created" content="2015-07-22T09:00:00-08:00" />
  </head>
  <body>
    <p>Here's an image from an <i>online source</i>:</p>
    <img src="https://..." alt="an image on the page" width="500" />
    <p>Here's an image uploaded as <b>binary data</b>:</p>
    <img src="name:imageBlock1" alt="an image on the page" width="300" />
    <p>Here's a file attachment:</p>
    <object data-attachment="FileName.pdf" data="name:fileBlock1" type="application/pdf" />
  </body>
</html>

--MyPartBoundary198374
Content-Disposition:form-data; name="imageBlock1"
Content-Type:image/jpeg

... binary image data ...

--MyPartBoundary198374
Content-Disposition:form-data; name="fileBlock1"
Content-Type:application/pdf

... binary file data ...

--MyPartBoundary198374--
```

Para obter mais exemplos que mostram como criar páginas que contêm imagens e outros arquivos, consulte [Adicionar imagens e arquivos](onenote-images-files.md), nossos [tutoriais](/previous-versions/office/office-365-api/how-to/onenote-tutorial) e nossos [exemplos](https://github.com/onenotedev). Além disso, saiba como [criar elementos posicionados absolutos](onenote-abs-pos.md), [usar marcas de anotação](onenote-note-tags.md) e [extrair dados](onenote-extract-data.md) para capturas de cartão de visita e as listagens online de receitas e de produtos.

O Microsoft Graph é rigoroso com certos formatos, como novas linhas CRLF em um corpo da mensagem de diversas partes. Para reduzir o risco de criar cargas mal formadas, você deve usar uma biblioteca para criar mensagens de diversas partes. 

Se você receber o status 400 para uma carga mal formada, verifique a formatação de novas linhas e espaços em branco e verifique se há problemas de codificação. Por exemplo, tente usar `charset=utf-8` (exemplo: `Content-Type: text/html; charset=utf-8`).

Consulte [Requisitos e limitações do HTML de entrada](#requirements-and-limitations-for-input-html-in-post-pages-requests) e [Limites de tamanho para solicitações POST](onenote-images-files.md#size-limitations-for-post-pages-requests).


<a name="request-response-info"></a>

## <a name="request-and-response-information-for-post-pages-requests"></a>Informações de solicitação e resposta para solicitações de *páginas POST* 

| Dados da solicitação | Descrição |  
|------|------|  
| Protocolo | Todas as solicitações usam o protocolo HTTPS de SSL/TLS. |  
| Cabeçalho de autorização | <p>`Bearer {token}`, onde `{token}` é um token de acesso do OAuth 2.0 válido para o aplicativo registrado.</p><p>Se ele estiver ausente ou for inválido, a solicitação falhará com um código de status 401. Confira [Autenticação e permissões](permissions-reference.md).</p> |  
| Cabeçalho content-type | <p>`text/html` ou `application/xhtml+xml` para o conteúdo HTML, seja enviado diretamente no corpo da mensagem, seja na parte "Apresentação" obrigatória de solicitações de diversas partes.</p><p>As solicitações de diversas partes são necessárias quando se enviam dados binários e usam o tipo de conteúdo `multipart/form-data; boundary=part-boundary`, onde `{part-boundary}` é uma cadeia de caracteres que sinaliza o início e o término de cada parte de dados.</p> |  
| Cabeçalho Accept | `application/json` | 

<br/>

| Dados de resposta | Descrição |  
|------|------|  
| Código de êxito | Um código de status HTTP 201. |  
| Corpo da resposta | Uma representação OData da nova página no formato JSON. |  
| Erros | Se a solicitação falhar, a API retornará erros no objeto **\@@api.diagnostics** no corpo da resposta. |  
| Cabeçalho location | A URL do recurso para a nova página. |  
| Cabeçalho X-CorrelationId | Um GUID que identifica de forma exclusiva a solicitação. Você pode usar esse valor juntamente com o valor do cabeçalho Data ao trabalhar com o suporte da Microsoft para solucionar problemas. |  


<a name="root-url"></a>

### <a name="constructing-the-microsoft-graph-service-root-url"></a>Criar a URL raiz do serviço do Microsoft Graph

A URL raiz do serviço do Microsoft Graph usa o formato a seguir para todas as chamadas para o Microsoft Graph:

`https://graph.microsoft.com/{version}/me/onenote/`  

O segmento `version` na URL representa a versão do Microsoft Graph que você deseja usar. Use `v1.0` para o código de produção estável. Use `beta` para experimentar um recurso que está em desenvolvimento. Os recursos e a funcionalidade na versão beta podem mudar, por isso, você não deve usá-la no código de produção. 

Use `me` para o conteúdo do OneNote que o usuário atual pode acessar (exclusivo e compartilhado). Use `users/{id}` para o conteúdo do OneNote que o usuário especificado (na URL) compartilhou com o usuário atual. Use o [Microsoft Graph](https://graph.microsoft.com/v1.0/users) para obter as IDs de usuário. 

<a name="limitations"></a>

## <a name="onenote-section-size-limitations"></a>Limitações de tamanho de seção do OneNote
Há um limite para o número de páginas que você pode adicionar a uma seção usando a API do OneNote. Quando esse limite é atingido em uma seção e é feita uma tentativa de criar uma nova página nessa seção, você verá uma resposta com o código de status HTTP `507` e a mensagem "O número máximo de páginas permitido por seção foi excedido". Para obter mais informações sobre esse código de erro, consulte [Códigos de erro do OneNote](onenote-error-codes.md).

Você pode usar uma das seguintes soluções alternativas:
- Crie uma nova seção e adicione novas páginas.
- Exclua páginas não utilizadas de uma seção existente que atingiu o limite de páginas.

<a name="permissions"></a>

## <a name="permissions"></a>Permissões

Para criar páginas do OneNote, solicite as permissões apropriadas. Escolha o nível mais baixo de permissões que seu aplicativo precisa para realizar o trabalho.

Escolha entre:

- Notes.Create
- Notes.ReadWrite
- Notes.ReadWrite.All

Para saber mais sobre escopos de permissão e como eles funcionam, confira [Referência de permissões do Microsoft Graph](permissions-reference.md).




<a name="see-also"></a>

## <a name="see-also"></a>Confira também

- [Adicionar imagens e arquivos](onenote-images-files.md)
- [Criar elementos posicionados absolutos](onenote-abs-pos.md)  
- [Extrair dados](onenote-extract-data.md)
- [Usar marcas de anotação](onenote-note-tags.md)
- [Integrar com o OneNote](integrate-with-onenote.md)
- [Blog de desenvolvedor do OneNote](https://go.microsoft.com/fwlink/?LinkID=390183)
- [Perguntas de desenvolvimento do OneNote no Microsoft Q&A](https://docs.microsoft.com/answers/topics/microsoft-graph-notes.html)
- [Repositórios do OneNote no GitHub](https://go.microsoft.com/fwlink/?LinkID=390178)