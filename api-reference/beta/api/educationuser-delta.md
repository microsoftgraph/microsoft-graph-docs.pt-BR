---
title: 'educationUser: Delta'
description: Obter usuários recém-criados ou atualizados sem ter que realizar uma leitura completa de toda a coleção de usuários.
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: d0952c9957395b21c20ace30fc1f800a526934e9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955275"
---
# <a name="educationuser-delta"></a>educationUser: Delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Obter [educationUser](../resources/educationuser.md) recentemente criados ou atualizados sem ter que realizar uma leitura completa de toda a coleção. Consulte [usar a consulta Delta](/graph/delta-query-overview) para obter detalhes.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | EduRoster. ReadBasic, EduRoster. Read ou EduRoster. ReadWrite              |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                                           |
| Application                            | EduRoster. ReadBasic. All, EduRoster. Read. All ou EduRoster. WriteWrite. All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /education/users/delta
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
| :------------ | :------------ |
| Authorization | Portador {código} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto da coleção [educationUser](../resources/educationuser.md) no corpo da resposta.

> [!IMPORTANT]
> educationUser deltas não incluem usuários excluídos.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationuser_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/users/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationuser-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationuser-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationuser-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationuser-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1039

{
  "value": [
    {
      "accountEnabled": true,
      "assignedLicenses": [{ "@odata.type": "microsoft.graph.assignedLicense" }],
      "assignedPlans": [{ "@odata.type": "microsoft.graph.assignedPlan" }],
      "businessPhones": ["String"],
      "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
      "department": "String",
      "displayName": "String",
      "externalSource": "string",
      "givenName": "String",
      "id": "String (identifier)",
      "mail": "String",
      "mailNickname": "String",
      "mailingAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
      "middleName": "String",
      "mobilePhone": "String",
      "officeLocation": "String",
      "onPremisesInfo": {
        "@odata.type": "microsoft.graph.educationOnPremisesInfo"
      },
      "passwordPolicies": "String",
      "passwordProfile": { "@odata.type": "microsoft.graph.passwordProfile" },
      "preferredLanguage": "String",
      "primaryRole": "string",
      "provisionedPlans": [{ "@odata.type": "microsoft.graph.provisionedPlan" }],
      "residenceAddress": { "@odata.type": "microsoft.graph.physicalAddress" },
      "student": { "@odata.type": "microsoft.graph.educationStudent" },
      "surname": "String",
      "teacher": { "@odata.type": "microsoft.graph.educationTeacher" },
      "usageLocation": "String",
      "userPrincipalName": "String",
      "userType": "String"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationUser: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


