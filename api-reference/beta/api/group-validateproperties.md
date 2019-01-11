---
title: 'grupo: validateProperties'
description: Valide se apelido de nome ou email de exibição de um grupo Office 365 está em conformidade com as políticas de nomenclatura. Os clientes podem usar a API para determinar se um nome para exibição ou apelido de email é válido antes de tentar **Atualizar** um grupo do Office 365. Para validar as propriedades antes de criar um grupo, use a função de validateProperties para objetos de diretório.
localization_priority: Normal
ms.openlocfilehash: 0ffdf44f687ad047d952e00c268239432244006d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833898"
---
# <a name="group-validateproperties"></a>grupo: validateProperties

Valide se apelido de nome ou email de exibição de um grupo Office 365 está em conformidade com as políticas de nomenclatura. Os clientes podem usar a API para determinar se um nome para exibição ou apelido de email é válido antes de tentar **Atualizar** um grupo do Office 365. Para validar as propriedades antes de criar um grupo, use a [função validateProperties](directoryobject-validateproperties.md) para objetos de diretório.

As validações a seguintes são executadas para as propriedades de apelido de email e o nome de exibição: 
1. Validar os prefixos e sufixos de diretiva de nomenclatura
2. Validar a política de palavras proibidos personalizadas

Essa API retorna com a primeira falha encontrada. Se uma ou mais propriedades falharem validações vários, apenas a propriedade com a primeira falha de validação será retornada. No entanto, você pode validar o apelido de email e o nome para exibição e receber uma coleção de erros de validação, se você estiver validando somente os prefixos e sufixos de diretiva de nomenclatura.

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Group.Read.All, Group.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Group.Read.All, Group.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
``` http
POST /groups/<id>/validateProperties
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
|displayName|Cadeia de caracteres| O nome de exibição do grupo para validar. A propriedade não é necessária individualmente. No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária. |
|mailNickname|Cadeia de caracteres| O apelido de email do grupo para validar. A propriedade não é necessária individualmente. No entanto, pelo menos uma propriedade (displayName ou mailNickname) é necessária. |
|onBehalfOfUserId|Guid| A ID de objeto do usuário para representar ao chamar a API. Os resultados de validação são para os atributos e funções de onBehalfOfUserId. |

## <a name="response"></a>Resposta
Se tiver êxito e não houver nenhum erro de validação, o método retornará `204 No Content` código de resposta. Ele não retornará nada no corpo da resposta.

Se a solicitação for inválida, o método retornará `400 Bad Request` código de resposta. Uma mensagem de erro com detalhes sobre a solicitação inválida é retornada no corpo da resposta.

Se houver um erro de validação. O método retornará `422 Unprocessable Entity` código de resposta. Uma mensagem de erro e uma coleção de detalhes do erro será retornado no corpo da resposta.

## <a name="examples"></a>Exemplos

Este é um exemplo de uma solicitação de validação bem-sucedida.

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "group_validateproperties"
}-->
``` http
POST https://graph.microsoft.com/beta/groups/{id}/validateProperties
Content-type: application/json
Content-length: 132

{
  "displayName": "Myprefix_test_mysuffix",
  "mailNickname": "Myprefix_test_mysuffix",
  "onBehalfOfUserId": "onBehalfOfUserId-value"
}
```

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
Content-length: 128

{
  "displayName": "MyPrefix_test_mysuffix",
  "mailNickname": "MyPrefix_test_mysuffix"
}
```

### <a name="response"></a>Resposta
```http
HTTP/1.1 422
Content-type: application/json
Content-length: 223

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
  "tocPath": ""
}-->
