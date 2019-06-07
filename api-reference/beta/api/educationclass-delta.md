---
title: 'educationClass: Delta'
description: Obter classes recém-criadas ou atualizadas, incluindo as alterações de associação, sem ter que realizar uma leitura completa de toda a coleção de classes.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 03a026a479c9502e00b86e41936619613013b9af
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764723"
---
# <a name="educationclass-delta"></a>educationClass: Delta

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter classes recém-criadas ou atualizadas, incluindo as alterações de associação, sem ter que realizar uma leitura completa de toda a coleção de classes. Consulte [usar a consulta Delta](/graph/delta-query-overview) para obter detalhes.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | EduRoster. ReadBasic, EduRoster. Read ou EduRoster. ReadWrite              |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                                           |
| Aplicativo                            | EduRoster. ReadBasic. All, EduRoster. Read. All ou EduRoster. WriteWrite. All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /education/classes/{id}/delta
POST /education/me/classes/{id}/delta
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
| :------------ | :------------ |
| Authorization | Portador {código} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto da coleção [educationClass](../resources/educationclass.md) no corpo da resposta.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra como chamar essa API.

##### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

<!-- {
  "blockType": "request",
  "name": "educationclass_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/classes/{id}/delta
```

##### <a name="response"></a>Resposta

Este é um exemplo de resposta. 

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

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
      "displayName": "displayName-value",
      "mailNickname": "mailNickname-value",
      "description": "description-value",
      "createdBy": {
        "application": {
          "displayName": "displayName-value",
          "id": "id-value"
        },
        "device": {
          "displayName": "displayName-value",
          "id": "id-value"
        },
        "user": {
          "displayName": "displayName-value",
          "id": "id-value"
        }
      },
      "classCode": "classCode-value",
      "externalName": "externalName-value"
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
