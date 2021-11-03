---
author: swapnil1993
title: 'site: getApplicableContentTypesForList'
description: Obter tipos de conteúdo de site que podem ser adicionados a uma lista.
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: ec0e453973c825da8ac6ed13094984a63ae71f88
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730400"
---
# <a name="site-getapplicablecontenttypesforlist"></a>site: getApplicableContentTypesForList
Namespace: microsoft.graph



Obter [][] [contentTypes][contentType] de site que podem ser adicionados a uma lista.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Sites.Read.All, Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/getApplicableContentTypesForList
```

## <a name="function-parameters"></a>Parâmetros de função
Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.
A tabela a seguir mostra os parâmetros que podem ser usados com esta função.

|Parâmetro|Tipo|Descrição|
|-|-|-|
|listId| String | GUID da lista para a qual os tipos de conteúdo aplicáveis precisam ser buscados. Obrigatório. |

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

Para listar apenas tipos de conteúdo personalizados, use `$filter=isBuiltin eq false` .

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [contentType](../resources/contenttype.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "site_getapplicablecontenttypesforlist"
}
-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/sites/{siteId}/getApplicableContentTypesForList(listId='{listId}')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/site-getapplicablecontenttypesforlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/site-getapplicablecontenttypesforlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/site-getapplicablecontenttypesforlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/site-getapplicablecontenttypesforlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contentType",
  "isCollection": true
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
        "id":"0x",
        "description":"",
        "group":"_Hidden",
        "hidden":false,
        "name":"System",
        "base": {
            "name": "System",
            "id": "0x"
        }
    },
    {
        "id":"0x00A7470EADF4194E2E9ED1031B61DA0884",
        "name": "docSet",
        "description": "custom docset",
        "hidden":false,
        "base": {
            "name": "Document Set",
            "id": "0x0120D520"
        },
        "group": "Custom Content Types"
    }
  ]
}
```

[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
