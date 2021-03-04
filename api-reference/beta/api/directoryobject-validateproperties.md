---
title: 'directoryObject: validateProperties'
description: Valide se o nome de exibição ou apelido de email de um grupo da Microsoft 365 está em conformidade com as políticas de nomenclatura.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 699175bfd3d51deb07d64722a7196fcf9dcc8880
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436831"
---
# <a name="directoryobject-validateproperties"></a>directoryObject: validateProperties

Namespace: microsoft.graph

Valide se o nome de exibição ou apelido de email de um grupo da Microsoft 365 está em conformidade com as políticas de nomenclatura.  Os clientes podem usar essa API para determinar se um nome de exibição ou apelido de email é válido antes de tentar **criar** um grupo do Microsoft 365. Para validar propriedades de um grupo existente, use a [função validateProperties](group-validateproperties.md) para grupos.

As seguintes validações são executadas para as propriedades nome de exibição e apelido de email: 
1. Validar a política de nomeação de prefixo e sufixo
2. Validar a política de palavras proibidas personalizada
3. Validar o apelido de email é exclusivo

Essa API retorna com a primeira falha encontrada. Se uma ou mais propriedades falharem em várias validações, somente a propriedade com a primeira falha de validação será retornada. No entanto, você pode validar o apelido de email e o nome de exibição e receber uma coleção de erros de validação se estiver validando apenas a política de nomenis de prefixo e sufixo.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           | Descrição      |
|:---------------|:-----------------|
| Autorização  | Portador {código}. Obrigatório.   |
| Content-Type   | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|entityType|String| `Group` é o único tipo de entidade com suporte. |
|displayName|String| O nome de exibição do grupo a ser validado. A propriedade não é necessária individualmente. No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária. |
|mailNickname|String| O apelido de email do grupo a ser validado. A propriedade não é necessária individualmente. No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária. |
|onBehalfOfUserId|Guid| A ID do objeto do usuário a ser personificado ao chamar a API. Os resultados da validação são para os atributos e funções de onBehalfOfUserId. |

## <a name="response"></a>Resposta

Se tiver êxito e não houver erros de validação, o método retornará `204 No Content` o código de resposta. Não retorna nada no corpo da resposta.

Se a solicitação for inválida, o método retornará `400 Bad Request` o código de resposta. Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.

Se houver um erro de validação, o método retornará `422 Unprocessable Entity` o código de resposta. Uma mensagem de erro e uma coleção de detalhes de erro é retornada no corpo da resposta.

## <a name="examples"></a>Exemplos

Este é um exemplo de uma solicitação de validação bem-sucedida.

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-validateproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-validateproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-validateproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-validateproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

Este é um exemplo de uma solicitação com erros de validação.

### <a name="request"></a>Solicitação
```http
POST https://graph.microsoft.com/beta/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "test",
  "mailNickname": "test",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

### <a name="response"></a>Resposta
```http
HTTP/1.1 422 
Content-Type: application/json

{
  "error": {
    "code": "Request_UnprocessableEntity",
    "message": "The values provided contain one or more validation errors.",
    "innerError": {
      "request-id": "request-id-value",
      "date": "date-value"
    },
    "details": [
      {
        "target": "displayName",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      },
      {
        "target": "mailNickname",
        "code": "MissingPrefixSuffix",
        "message": "Property mailNickname is missing a required prefix/suffix per your organization's Group naming requirements.",
        "prefix": "Myprefix_",
        "suffix": "_mysuffix"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: validateProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


