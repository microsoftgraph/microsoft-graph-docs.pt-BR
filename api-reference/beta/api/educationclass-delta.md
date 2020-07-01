---
title: 'educationClass: Delta'
description: Obter classes recém-criadas ou atualizadas, incluindo as alterações de associação, sem ter que realizar uma leitura completa de toda a coleção de classes.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 0b22ca9852d89c0d80d52959cef99c68fcc43bb8
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006846"
---
# <a name="educationclass-delta"></a>educationClass: Delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter classes recém-criadas ou atualizadas, incluindo as alterações de associação, sem ter que realizar uma leitura completa de toda a coleção de classes. Consulte [usar a consulta Delta](/graph/delta-query-overview) para obter detalhes.

## <a name="permissions"></a>Permissões

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| Delegada (conta corporativa ou de estudante)     | EduRoster. ReadBasic, EduRoster. Read ou EduRoster. ReadWrite              |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                                                           |
| Application                            | EduRoster. ReadBasic. All, EduRoster. Read. All ou EduRoster. WriteWrite. All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /education/classes/delta
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
| :------------ | :------------ |
| Authorization | Portador {código} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto da coleção [educationClass](../resources/educationclass.md) no corpo da resposta.

> [!IMPORTANT]
> educationClass deltas não incluem classes excluídas.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}-->

```http
GET https://graph.microsoft.com/beta/education/classes/delta
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 585

{
  "value": [
    {
      "classCode": "String",
      "course": { "@odata.type": "microsoft.graph.educationCourse" },
      "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
      "description": "String",
      "displayName": "String",
      "externalId": "String",
      "externalName": "String",
      "externalSource": "string",
      "grade": "string",
      "id": "String (identifier)",
      "mailNickname": "String",
      "term": { "@odata.type": "microsoft.graph.educationTerm" }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
