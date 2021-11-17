---
author: swapnil1993
title: Criar um tipo de conteúdo
description: Crie um tipo de conteúdo em um site.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: d36ef7694344aab8c774467d18a1595fe6f5b8de
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61027113"
---
# <a name="create-a-content-type"></a>Criar um tipo de conteúdo
Namespace: microsoft.graph

Criar um novo [contentType][] em um [site][].

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |Sites.Manage.All, Sites.FullControl.All    |
|Delegado (conta pessoal da Microsoft) |Não suportado    |
|Aplicativo |Sites.Manage.All, Sites.FullControl.All |


## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{site-id}/contentTypes
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [recurso contentType][] a ser criado.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [contentType][] no corpo da resposta.


## <a name="example"></a>Exemplo

O exemplo a seguir mostra como criar um novo tipo de conteúdo genérico.

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_contenttype"
}
-->

```http
POST https://graph.microsoft.com/v1.0/sites/{id}/contentTypes
Content-Type: application/json

{
    "name": "docSet",
    "description": "custom docset",
    "base": {
        "name": "Document Set",
        "id": "0x0120D520"
    },
    "group": "Document Set Content Types" 
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-contenttype-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType"
}
-->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "0x01002A2479FF33DD4BC3B1533A012B653717",
  "name": "docSet",
  "group":"Document Set Content Types",
  "description" : "custom docset",
  "base": {
        "name": "Document Set",
        "id": "0x0120D520"
   }
}
```


[contentType]: ../resources/contentType.md
[site]: ../resources/site.md

<!--
{
  "type": "#page.annotation",
  "description": "Create a content type in a site",
  "keywords": "content type",
  "section": "documentation",
  "tocPath": "sites/Create ContentType",
  "suppressions": [
  ]
}
-->
