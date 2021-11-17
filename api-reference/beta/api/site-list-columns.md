---
author: swapnil1993
title: Listar colunas em um site
description: Listar colunas em um site.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: a1ef129c44a2094468e4ba30f775cfd7abccb3cb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61026175"
---
# <a name="list-columns-in-a-site"></a>Listar colunas em um site
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
Obter o conjunto de colunas, representado como [columnDefinition][columnDefinition] resources, in a [site][site].

  

## <a name="permissions"></a>Permissões

  

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

  

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All  |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo | Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All  |

  

## <a name="http-request"></a>Solicitação HTTP

  
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /sites/{site-id}/columns
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

Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos columnDefinition][] no corpo da resposta.

  

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- { "blockType": "request", "name": "get_columns_from_site" } -->
 

```msgraph-interactive
GET https://graph.microsoft.com/beta/sites/{site-id}/columns
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-columns-from-site-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-columns-from-site-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-columns-from-site-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-columns-from-site-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-columns-from-site-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.columnDefinition)"
}
-->  

```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "value":[
      {
         "description":"",
         "displayName":"Title",
         "hidden":false,
         "id":"99ddcf45-e2f7-4f17-82b0-6fba34445103",
         "indexed":false,
         "name":"Title",
         "readOnly":false,
         "required":false,
         "text":{
            "allowMultipleLines":false,
            "appendChangesToExistingText":false,
            "linesForEditing":0,
            "maxLength":255
         }
      },
      {
         "description":"",
         "displayName":"Address",
         "id":"11dfef35-e2f7-4f17-82b0-6fba34445103",
         "indexed":false,
         "name":"Address",
         "readOnly":false,
         "required":false,
         "text":{
            "allowMultipleLines":false,
            "appendChangesToExistingText":false,
            "linesForEditing":0,
            "maxLength":255
         }
      }
   ]
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[site]: ../resources/site.md
 
