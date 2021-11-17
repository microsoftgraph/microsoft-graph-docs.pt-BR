---
title: 'group: validateProperties'
description: Valide se Microsoft 365 nome de exibição de um grupo ou apelido de email estiver em conformidade com as políticas de nomenização.
ms.localizationpriority: medium
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 4cc1aa6a36a0e270313c1654814149ee3e8d5ce4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61015067"
---
# <a name="group-validateproperties"></a>group: validateProperties

Namespace: microsoft.graph

Valide se Microsoft 365 nome de exibição de um grupo ou apelido de email estiver em conformidade com as políticas de nomenização. Os clientes podem usar **a** API para determinar se um nome de exibição ou apelido de email é válido antes de tentar atualizar um Microsoft 365 grupo. Para validar propriedades antes de criar um grupo, use a [função validateProperties](directoryobject-validateproperties.md) para objetos de diretório.

As seguintes validações são executadas para as propriedades nome de exibição e apelido de email: 
1. Validar a política de nomeação de prefixo e sufixo
2. Validar a política de palavras proibidas personalizada

Essa API retorna com a primeira falha encontrada. Se uma ou mais propriedades falharem em várias validações, somente a propriedade com a primeira falha de validação será retornada. No entanto, você pode validar o apelido de email e o nome de exibição e receber uma coleção de erros de validação se estiver validando apenas a política de nomenis de prefixo e sufixo.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.Read.All, Group.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Group.Read.All, Group.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/{id}/validateProperties
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           | Descrição      |
|:---------------|:-----------------|
| Authorization  | Portador {código}    |
| Content-Type   | application/json |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|String| O nome de exibição do grupo a ser validado. A propriedade não é necessária individualmente. No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária. |
|mailNickname|String| O apelido de email do grupo a ser validado. A propriedade não é necessária individualmente. No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária. |
|onBehalfOfUserId|Guid| A ID do objeto do usuário a ser personificado ao chamar a API. Os resultados da validação são para os atributos e funções de onBehalfOfUserId. |

## <a name="response"></a>Resposta
Se tiver êxito e não houver erros de validação, o método retornará `204 No Content` o código de resposta. Não retorna nada no corpo da resposta.

Se a solicitação for inválida, o método retornará `400 Bad Request` o código de resposta. Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.

Se houver um erro de validação. O método retorna `422 Unprocessable Entity` o código de resposta. Uma mensagem de erro e uma coleção de detalhes de erro é retornada no corpo da resposta.

## <a name="examples"></a>Exemplos

Este é um exemplo de uma solicitação de validação bem-sucedida.

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/group-validateproperties-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

Este é um exemplo de uma solicitação com erros de validação.

### <a name="request"></a>Solicitação
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a>Resposta
```http
HTTP/1.1 422
Content-type: application/json

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "mailNickname",
        "code": "PropertyConflict",
        "message": "Another object with the same value for property mailNickname already exists."
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


