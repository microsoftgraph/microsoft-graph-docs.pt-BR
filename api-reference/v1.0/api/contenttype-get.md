---
author: swapnil1993
title: Obter contentType
description: Obter um tipo de conteúdo em um site ou em uma lista.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 4f0886b63061a6996dda7559b3c53ce6187d0486
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101351"
---
# <a name="get-contenttype"></a>Obter contentType
Namespace: microsoft.graph



Recupere os metadados de [um tipo de conteúdo][contentType] em um [site][] ou em uma [lista][].

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/contentTypes/{contentType-id}

GET /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [contentType](../resources/contenttype.md) no corpo da resposta.


## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contenttype"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/{contentType-id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contenttype-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contenttype-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contenttype-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contenttype-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-contenttype-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-contenttype-powershell-snippets.md)]
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
HTTP/1.1 200 OK
Content-type: application/json

{
  "id":"0x0120D520",
  "description":"Create a document set when you want to manage multiple documents as a single work product.",
  "group":"Document Set Content Types",
  "hidden":false,
  "name":"Document Set",
  "base": {
        "name": "Document Set",
        "id": "0x0120D520"
   }
}
```

[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
[list]: ../resources/list.md
