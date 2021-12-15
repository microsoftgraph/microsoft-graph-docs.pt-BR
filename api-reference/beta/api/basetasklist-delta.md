---
title: 'baseTaskList: delta'
description: Obter um conjunto de recursos baseTaskList que foram adicionados, excluídos ou removidos em Microsoft To Do.
author: devindrajit
ms.localizationpriority: medium
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2448a287cd3b36edad9c338899d366e69c1685d6
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525243"
---
# <a name="basetasklist-delta"></a>baseTaskList: delta
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter um conjunto de [recursos baseTaskList](../resources/basetasklist.md) que foram adicionados, excluídos ou removidos em Microsoft To Do.

Uma **chamada** de função delta para **baseTaskList** é semelhante a uma solicitação GET, exceto que, aplicando adequadamente [tokens](/graph/delta-query-overview) de estado em uma ou mais dessas chamadas, você pode consultar alterações incrementais na **baseTaskList**. Isso permite manter e sincronizar um armazenamento local de **baseTaskList** de um usuário sem precisar buscar todas as **baseTaskList** do servidor sempre.

## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Tasks.Read, Tasks.ReadWrite|
|Delegada (conta pessoal da Microsoft)|Tasks.Read, Tasks.ReadWrite|
|Aplicativo|Sem suporte|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/tasks/lists/delta
GET /users/{userId|userPrincipalName}/tasks/lists/delta
```

## <a name="query-parameters"></a>Parâmetros de consulta

Controlar alterações nos **recursos baseTaskList** incorre em uma rodada de uma ou mais chamadas de **função delta.** Se você usar qualquer parâmetro de consulta (diferente de `$deltatoken` e `$skiptoken`), especifique-o na primeira solicitação **delta**. O Microsoft Graph codifica automaticamente todos os parâmetros especificados na parte do token da URL `nextLink` ou `deltaLink` fornecida na resposta. Você só precisa especificar uma vez os parâmetros de consulta desejados antecipadamente. Em solicitações subsequentes, basta copiar e aplicar a URL ou da resposta anterior, pois essa URL já inclui os `nextLink` `deltaLink` parâmetros codificados e desejados.

| Parâmetro de consulta    | Tipo |Descrição|
|:---------------|:--------|:----------|
| $deltatoken | string | Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior para a mesma coleção `deltaLink` **baseTaskList,** indicando a conclusão dessa rodada de controle de alterações.  Salve e aplique toda a URL `deltaLink`, incluindo esse token na primeira solicitação da próxima série de controle de alterações desse conjunto.|
| $skiptoken | string | Um [token de estado](/graph/delta-query-overview) retornado na URL da chamada de função delta anterior, indicando que há outras alterações a serem controladas na mesma coleção `nextLink` **baseTaskList.**  |

### <a name="odata-query-parameters"></a>Parâmetros de consulta OData

- Suporte à consulta delta e parâmetros de consulta `$filter` `$top` para `$expand` **baseTaskList**. 
- Não há suporte para `$search`. 

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição |
|:---------------|:----------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |
| Preferir | cadeia de caracteres  | odata.maxpagesize={x}. Opcional. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará um código `200 OK` de resposta e uma coleção [baseTaskList](../resources/basetasklist.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "basetasklist_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/tasks/lists/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/basetasklist-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/basetasklist-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/basetasklist-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/basetasklist-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.baseTaskList)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(baseTaskList)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/tasks/lists/delta?$skiptoken=AVCnFFj2r7PtnjtkD-g_6Y5Ntek1m4V",
    "value": [
        {
            "@odata.type": "#microsoft.graph.wellKnownTaskList",
            "@odata.etag": "W/\"kOO4xOT//0qFRAqk3TNe0QAAAAAAkw==\"",
            "wellKnownListName": "defaultList",
            "displayName": "Tasks",
            "id": "AQMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNm"
        }
    ]
}
```

