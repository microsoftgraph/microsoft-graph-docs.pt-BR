---
title: Listar itens excluídos
description: Recupere uma lista de itens recentemente excluídos em itens excluídos.
author: keylimesoda
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3071e92cc17aa15e111c1483d9a1092a3ddc91dd
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226248"
---
# <a name="list-deleted-items"></a>Listar itens excluídos

Namespace: microsoft.graph

Recupere uma lista de itens recentemente excluídos em [itens excluídos](../resources/directory.md).

Atualmente, a funcionalidade de itens excluídos só tem suporte para os recursos [de](../resources/application.md)aplicativo, [grupo](../resources/group.md) [e](../resources/user.md) usuário.

## <a name="permissions"></a>Permissões

[!INCLUDE [limited-info](../../includes/limited-info.md)]

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

### <a name="for-applications"></a>Para aplicativos:

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Application.Read.All, Application.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Application.Read.All, Application.ReadWrite.All, Directory.Read.All |

### <a name="for-users"></a>Para usuários:

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo | User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

### <a name="for-groups"></a>Para grupos:

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Group.Read.All, Group.ReadWrite.All, Directory.Read.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.application
GET /directory/deletedItems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
GET /directory/deletedItems/microsoft.graph.device
```

Atualmente, essa API dá suporte à recuperação de tipos de objeto de aplicativos ( `microsoft.graph.application` ), grupos ( ) ou usuários ( ) de itens `microsoft.graph.group` `microsoft.graph.user` excluídos. O tipo de cast OData é uma parte necessária do URI e não há suporte para chamada sem `GET /directory/deleteditems` um tipo. 

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Este método dá suporte aos parâmetros de consulta compatíveis com o recurso especificado pelo cast OData. Ou seja, `$count` , , , , , e `$expand` `$filter` `$orderBy` `$search` `$select` `$top` parâmetros de consulta. Algumas consultas são suportadas somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`. Por exemplo:

```msgraph-interactive
https://graph.microsoft.com/beta/directory/deletedItems/microsoft.graph.group?&$count=true&$orderBy=deletedDateTime desc&$select=id,displayName,deletedDateTime
ConsistencyLevel: eventual
```

Este exemplo requer o header **ConsistencyLevel** porque os parâmetros e de consulta `$orderBy` são usados na `$count` consulta.

### <a name="examples-using-the-orderby-odata-query-parameter"></a>Exemplos usando o parâmetro $orderBy consulta OData

O parâmetro de consulta OData é suportado nas propriedades `$orderBy` **deletedDateTime**, **displayName** e **userPrincipalName** dos tipos de objeto excluídos. Na propriedade **deletedDateTime,** a consulta requer a adição dos parâmetros de consulta avançados ( Header **ConsistencyLevel** definido como e cadeia de [caracteres](/graph/aad-advanced-queries) `true` de `$count=true` consulta).

| OData cast | Propriedades que suportam $orderBy | Exemplo |
| :--- | :--- | :--- |
| microsoft.graph.user | deletedDateTime, displayName, userPrincipalName | /directory/deletedItems/microsoft.graph.user?$orderBy=userPrincipalName |
| microsoft.graph.group | deletedDateTime, displayName | /directory/deletedItems/microsoft.graph.group?$orderBy=deletedDateTime asc&$count=true |
| microsoft.graph.application | deletedDateTime, displayName | /directory/deletedItems/microsoft.graph.application?$orderBy=displayName |
| microsoft.graph.device | deletedDateTime, displayName | /directory/deletedItems/microsoft.graph.device?$orderBy=deletedDateTime&$count=true |

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome      |Descrição|
|:----------|:----------|
| Autorização  | &lt;Código&gt; do portador *Obrigatório*|
| Aceitar  | application/json |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.
## <a name="examples"></a>Exemplos

### <a name="example-1-retrieve-deleted-groups"></a>Exemplo 1: Recuperar grupos excluídos

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "ignored",
  "name": "get_deleteditems"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group
```

#### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

### <a name="example-2-retrieve-the-count-of-deleted-user-objects-and-order-the-results-by-the-deleteddatetime-property"></a>Exemplo 2: recupere a contagem de objetos de usuário excluídos e peça os resultados pela propriedade deletedDateTime

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_deleteditems_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/deletedItems/microsoft.graph.group?$count=true&$orderBy=deletedDateTime asc&$select=id,DisplayName,deletedDateTime
ConsistencyLevel: eventual
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-deleteditems-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-deleteditems-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-deleteditems-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-deleteditems-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-deleteditems-count-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups(id,displayName,deletedDateTime)",
    "@odata.count": 2,
    "value": [
        {
            "id": "c31799b8-0683-4d70-9e91-e032c89d3035",
            "displayName": "Role assignable group",
            "deletedDateTime": "2021-10-26T16:56:36Z"
        },
        {
            "id": "74e45ce0-a52a-4766-976c-7201b0f99370",
            "displayName": "Role assignable group",
            "deletedDateTime": "2021-10-26T16:58:37Z"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
