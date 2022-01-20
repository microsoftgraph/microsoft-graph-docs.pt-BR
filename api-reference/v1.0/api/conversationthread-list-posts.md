---
title: Listar postagens
description: 'Obtenha as postagens do thread especificado. Você pode especificar a conversa pai e o thread ou, '
ms.localizationpriority: medium
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e6dafa95621e69ed2a0263fce5a8036dad96a0b1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098027"
---
# <a name="list-posts"></a>Listar postagens

Namespace: microsoft.graph

Obtenha as postagens do thread especificado. Você pode especificar a conversa pai e o thread ou apenas o thread, sem fazer referência à conversa pai.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.Read.All, Group.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Group.Read.All, Group.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{groupId}/threads/{threadId}/posts
GET /groups/{groupId}/conversations/{conversationId}/threads/{threadId}/posts

```
## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte ao `$select` [parâmetro de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta. `$expand` também tem suporte para expandir relações específicas e apenas uma relação pode ser expandida em uma única solicitação.
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [Post](../resources/post.md) no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_posts"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/threads/AAQkADI5YzgxODgyLTExZDgtNDhkMS1iZDRjLTBhZGZiN2ExYWQxNwMkABAADW7fw6FZNEuyjrGA9R8SshAADW7fw6FZNEuyjrGA9R8Ssg==/posts
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-posts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-posts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-posts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-posts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-posts-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-posts-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Resposta
Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.post",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('02f3bafb-448c-487c-88c2-5fd65ce49a41')/threads('AAQkADI5YzgxODgyLTExZDgtNDhkMS1iZDRjLTBhZGZiN2ExYWQxNwMkABAADW7fw6FZNEuyjrGA9R8SshAADW7fw6FZNEuyjrGA9R8Ssg%3D%3D')/posts",
  "value": [
    {
      "@odata.etag": "W/\"CQAAABYAAACWM1XFF4buR6Xp/9aBq6+wAAAAAAEK\"",
      "id": "AAMkADI5YzgxODgyLTExZDgtNDhkMS1iZDRjLTBhZGZiN2ExYWQxNwBGAAAAAAAmtAlgzc6xQZmiHzuqNLQ8BwCWM1XFF4buR6Xp-9aBq6_wAAAAAAEMAACWM1XFF4buR6Xp-9aBq6_wAAAAAAk9AAA=",
      "createdDateTime": "2021-04-14T07:01:07Z",
      "lastModifiedDateTime": "2021-04-14T07:01:08Z",
      "changeKey": "CQAAABYAAACWM1XFF4buR6Xp/9aBq6+wAAAAAAEK",
      "categories": [],
      "receivedDateTime": "2021-04-14T07:01:07Z",
      "hasAttachments": false,
      "body": {
        "contentType": "html",
        "content": "<html><body><div><div style=\"direction:ltr;\"><table border=\"0\" cellspacing=\"0\" cellpadding=\"0\" id=\"x_bodyTable\" style=\"vertical-align:top;width:100%;height:100%;border-spacing:0;border-collapse:collapse;margin:0;padding:0;border-width:0;box-sizing:border-box;\"><tr style=\"vertical-align:top;margin:0;padding:0;border-width:0;box-sizing:border-box;\"><td id=\"x_bodyCell\" style=\"vertical-align:top;direction:ltr;width:100%;height:100%;margin:0;padding:0;border-width:0;box-sizing:border-box;\"><table border=\"0\" cellspacing=\"0\" cellpadding=\"0\" id=\"x_content\" style=\"font-family:Segoe UI,Tahoma,Microsoft Sans Serif,Verdana,sans-serif;vertical-align:top;border-spacing:0;border-collapse:collapse;margin:0;padding:0;border-width:0;box-sizing:border-box;\"><tr style=\"vertical-align:top;margin:0;padding:0;border-width:0;box-sizing:border-box;\"><td style=\"font-family:Segoe UI,Tahoma,Microsoft Sans Serif,Verdana,sans-serif;vertical-align:top;height:64px;margin:0;padding:0 0 20px 0;border-width:0;box-sizing:border-box;\"><div style=\"color:#0072C6;font-size:18pt;vertical-align:top;margin:0;padding:0;border-width:0;box-sizing:border-box;\">Welcome to the Contoso Life group...."
      },
      "from": {
        "emailAddress": {
          "name": "Contoso Life",
          "address": "contosolife@M365x435773.onmicrosoft.com"
        }
      },
      "sender": {
        "emailAddress": {
          "name": "Contoso Life",
          "address": "contosolife@M365x435773.onmicrosoft.com"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List posts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
