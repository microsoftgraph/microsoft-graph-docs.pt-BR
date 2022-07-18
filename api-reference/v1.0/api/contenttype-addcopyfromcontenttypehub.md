---
title: 'contentType: addCopyFromContentTypeHub'
description: Adicione ou sincronize uma cópia de um tipo de conteúdo publicado do hub de tipo de conteúdo para um site de destino ou uma lista.
author: swapnil1993
ms.localizationpriority: medium
ms.prod: sites-and-lists
doc_type: apiPageType
ms.openlocfilehash: e11553f5a7008802517d6f132437d2ebe7e07aeb
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444058"
---
# <a name="contenttype-addcopyfromcontenttypehub"></a>contentType: addCopyFromContentTypeHub
Namespace: microsoft.graph

Adicione ou sincronize uma cópia de um tipo de conteúdo publicado do hub de tipo de conteúdo para um [site de destino](../resources/site.md) ou uma [lista](../resources/list.md).

Esse método faz parte das alterações de publicação de tipo de conteúdo para otimizar a sincronização de tipos de conteúdo publicados para sites e listas, alternando efetivamente de uma abordagem "push everywhere" para "efetuar pull conforme necessário". O método permite que os usuários efetuem pull de tipos de conteúdo diretamente do hub de tipo de conteúdo para um site ou lista. Para obter mais informações, consulte [contentType: getCompatibleHubContentTypes](contenttype-getcompatiblehubcontenttypes.md) e a postagem no blog [Syntex Product Atualizações – agosto de 2021](https://techcommunity.microsoft.com/t5/sharepoint-syntex-blog/syntex-product-updates-august-2021/ba-p/2606438).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante) | Sites.Manage.All, Sites.FullControl.All |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sites.Manage.All, Sites.FullControl.All |


## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /sites/{siteId}/lists/{listId}/contentTypes/addCopyFromContentTypeHub
POST /sites/{siteId}/contentTypes/addCopyFromContentTypeHub
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra o parâmetro que pode ser usado com essa ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|Contenttypeid|Cadeia de caracteres| A ID do tipo de conteúdo no hub de tipo de conteúdo que será adicionado a um site de destino ou a uma lista.|



## <a name="response"></a>Resposta

Se tiver êxito, `200 OK` essa ação retornará um código de resposta e um objeto [contentType](../resources/contenttype.md) `202 Accepted` no corpo da resposta se o tipo de conteúdo for adicionado de forma síncrona ou um código de resposta se o tipo de conteúdo for sincronizado de forma assíncrona. A resposta também conterá um cabeçalho, que contém o local do [richLongRunningOperation](../resources/richlongrunningoperation.md) que foi criado para lidar com a `Location` operação de cópia/sincronização. No caso de uma operação assíncrona, pode levar até 70 minutos para sincronizar ou adicionar um tipo de conteúdo.

## <a name="examples"></a>Exemplos

### <a name="example-1-synchronous-pull"></a>Exemplo 1: pull síncrono

O exemplo a seguir adiciona ou sincroniza um tipo de conteúdo de forma síncrona com base em determinadas condições de back-end.

#### <a name="request"></a>Solicitação

A seguir está um exemplo de uma operação síncrona.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contenttype_addcopyfromcontenttypehub"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/sites/root/lists/Documents/contentTypes/addCopyFromContentTypeHub
Content-Type: application/json
Content-length: 33

{
  "contentTypeId": "0x0101"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contenttype-addcopyfromcontenttypehub-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contenttype-addcopyfromcontenttypehub-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contenttype-addcopyfromcontenttypehub-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/contenttype-addcopyfromcontenttypehub-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/contenttype-addcopyfromcontenttypehub-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/contenttype-addcopyfromcontenttypehub-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.contentType",
    "id": "0x0101",
    "description": "Document content type",
    "group": "Document Content Types",
    "hidden": false,
    "isBuiltIn": true,
    "name": "Document"
}
```

### <a name="example-2-asynchronous-pull"></a>Exemplo 2: pull assíncrono

O exemplo a seguir adiciona ou sincroniza um tipo de conteúdo de forma assíncrona porque as condições de back-end para uma operação síncrona não são atendidas.

#### <a name="request"></a>Solicitação

A seguir está um exemplo de uma operação assíncrona.

<!-- {
  "blockType": "request",
  "name": "contenttype_addcopyfromcontenttypehub"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/sites/root/lists/Documents/contentTypes/addCopyFromContentTypeHub
Content-Type: application/json
Content-length: 33

{
  "contentTypeId": "0x0101"
}
```


#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response"
}
-->
``` http
HTTP/1.1 202 Accepted
location: https://graph.microsoft.com/v1.0/sites/root/lists/Documents/operations/contentTypeCopy,0x0101
```
