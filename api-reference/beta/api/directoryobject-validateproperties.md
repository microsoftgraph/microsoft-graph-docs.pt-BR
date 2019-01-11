---
title: 'directoryObject: validateProperties'
description: Valide se apelido de nome ou email de exibição de um grupo Office 365 está em conformidade com as políticas de nomenclatura.  Os clientes podem usar a API para determinar se um nome para exibição ou apelido de email é válido antes de tentar **criar** um grupo do Office 365. Para validar as propriedades de um grupo existente, use a função validateProperties para grupos.
localization_priority: Normal
ms.openlocfilehash: 1f38a30d86cf5b28eea6b9891687c4dbca4b78fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879818"
---
# <a name="directoryobject-validateproperties"></a>directoryObject: validateProperties

Valide se apelido de nome ou email de exibição de um grupo Office 365 está em conformidade com as políticas de nomenclatura.  Os clientes podem usar a API para determinar se um nome para exibição ou apelido de email é válido antes de tentar **criar** um grupo do Office 365. Para validar as propriedades de um grupo existente, use a [função validateProperties](group-validateproperties.md) para grupos.

As validações a seguintes são executadas para as propriedades de apelido de email e o nome de exibição: 
1. Validar os prefixos e sufixos de diretiva de nomenclatura
2. Validar a política de palavras proibidos personalizadas
3. Validar o email apelido é exclusivo

Essa API retorna com a primeira falha encontrada. Se uma ou mais propriedades falharem validações vários, apenas a propriedade com a primeira falha de validação será retornada. No entanto, você pode validar o apelido de email e o nome para exibição e receber uma coleção de erros de validação, se você estiver validando somente os prefixos e sufixos de diretiva de nomenclatura.

## <a name="prerequisites"></a>Pré-requisitos

A seguinte **permissão** é necessária para executar essa API: *Group.Read.All*

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
``` http
POST /directoryObjects/validateProperties
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome           | Descrição      |
|:---------------|:-----------------|
| Autorização  | Portador {código}    |
| Content-Type   | application/json |

## <a name="request-body"></a>Corpo da solicitação
Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo   |Descrição|
|:---------------|:--------|:----------|
|entityType|Cadeia de caracteres| `Group`é o tipo de entidade com suporte apenas. |
|displayName|Cadeia de caracteres| O nome de exibição do grupo para validar. A propriedade não é necessária individualmente. No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária. |
|mailNickname|Cadeia de caracteres| O apelido de email do grupo para validar. A propriedade não é necessária individualmente. No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária. |
|onBehalfOfUserId|Guid| A ID de objeto do usuário para representar ao chamar a API. Os resultados de validação são para os atributos e funções de onBehalfOfUserId. |

## <a name="response"></a>Resposta

Se tiver êxito e não houver nenhum erro de validação, o método retornará `204 No Content` código de resposta. Ele não retornará nada no corpo da resposta.

Se a solicitação for inválida, o método retornará `400 Bad Request` código de resposta. Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.

Se houver um erro de validação, o método retornará `422 Unprocessable Entity` código de resposta. Uma mensagem de erro e uma coleção de detalhes do erro será retornado no corpo da resposta.

## <a name="examples"></a>Exemplos

Este é um exemplo de uma solicitação de validação bem-sucedida.

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "directoryobject_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/directoryObjects/validateProperties
Content-type: application/json
Content-length: 164

{
  "entityType": "Group",
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

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
POST https://graph.microsoft.com/directoryObjects/validateProperties
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
  "tocPath": ""
}-->
