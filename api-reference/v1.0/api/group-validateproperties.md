---
title: 'group: validateProperties'
description: Valide se o nome de exibição ou apelido de email de um grupo da Microsoft 365 está em conformidade com as políticas de nomenclatura.
ms.localizationpriority: medium
author: Jordanndahl
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: b3ae0e3153adf4ad5b466f3d7f79fdde082e2642
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60931624"
---
# <a name="group-validateproperties"></a>group: validateProperties

Namespace: microsoft.graph

Valide se o nome de exibição ou apelido de email de um grupo da Microsoft 365 está em conformidade com as políticas de nomenclatura.  Os clientes podem usar essa API para determinar se um nome de exibição ou apelido de email é válido antes de tentar atualizar [um](group-update.md) Microsoft 365 grupo. Para validar as propriedades antes de criar um grupo, use a [função directoryobject:validateProperties.](directoryobject-validateproperties.md)

As seguintes validações de política são executadas para as propriedades de nome de exibição e apelido de email:
1. Validar a política de nomeação de prefixo e sufixo
2. Validar a política de palavras proibidas personalizada

Essa API retorna apenas a primeira falha de validação encontrada. Se as propriedades falharem em várias validações, somente a primeira falha de validação será retornada. No entanto, você pode validar o apelido de email e o nome de exibição e receber uma coleção de erros de validação se estiver validando apenas a política de nomenis de prefixo e sufixo. Para saber mais sobre como configurar políticas de nomenização, consulte [Configure noming policy](/azure/active-directory/users-groups-roles/groups-naming-policy#configure-naming-policy-in-powershell).

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
| Autorização  | {token} de portador. Obrigatório.    |
| Content-Type   | application/json |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|displayName|Cadeia de caracteres| O nome de exibição do grupo a ser validado. A propriedade não é necessária individualmente. No entanto, pelo menos uma propriedade (**displayName** **ou mailNickname**) é necessária. |
|mailNickname|String| O apelido de email do grupo a ser validado. A propriedade não é necessária individualmente. No entanto, pelo menos uma propriedade (**displayName** **ou mailNickname**) é necessária. |
|onBehalfOfUserId|Guid| A ID do usuário a ser personificado ao chamar a API. Os resultados da validação são para os atributos e funções de **onBehalfOfUserId.** |

## <a name="response"></a>Resposta
Se tiver êxito e não houver erros de validação, o método retornará `204 No Content` o código de resposta. Não retorna nada no corpo da resposta.

Se a solicitação for inválida, o método retornará `400 Bad Request` o código de resposta. Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.

Se houver um erro de validação. O método retorna `422 Unprocessable Entity` o código de resposta. Uma mensagem de erro e uma coleção de detalhes de erro é retornada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-successful-validation-request"></a>Exemplo 1: Solicitação de validação bem-sucedida
Este é um exemplo de uma solicitação de validação bem-sucedida.

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
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

---


#### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-validation-errors"></a>Exemplo 2: Solicitação com erros de validação
Este é um exemplo de uma solicitação com erros de validação.

#### <a name="request"></a>Solicitação
``` http
POST https://graph.microsoft.com/v1.0/groups/{id}/validateProperties
Content-type: application/json

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

#### <a name="response"></a>Resposta
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

