---
title: 'educationSchool: delta'
description: Get newly created or updated schools without having to perform a full read of the entire school collection.
ms.localizationpriority: medium
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5c06a69ffae7f42e1da147f51c404852705e6d7a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60975184"
---
# <a name="educationschool-delta"></a>educationSchool: delta

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get newly created or updated schools without having to perform a full read of the entire school collection. Consulte [Usar consulta delta para](/graph/delta-query-overview) obter detalhes.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | EduRoster.ReadBasic, EduRoster.Read ou EduRoster.ReadWrite              |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                                                           |
| Aplicativo                            | EduRoster.ReadBasic.All, EduRoster.Read.All ou EduRoster.WriteWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /education/schools/delta
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
| :------------ | :------------ |
| Authorization | Portador {código} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto da coleção educationSchool](../resources/educationschool.md) no corpo da resposta.

> [!IMPORTANT]
> educationSchool deltas não incluem escolas excluídas.

## <a name="example"></a>Exemplo

O exemplo a seguir mostra como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/schools/delta
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/educationschool-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/educationschool-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/educationschool-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/educationschool-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/educationschool-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "address": { "@odata.type": "microsoft.graph.physicalAddress" },
      "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
      "description": "String",
      "displayName": "String",
      "externalId": "String",
      "externalPrincipalId": "String",
      "externalSource": "string",
      "highestGrade": "String",
      "id": "String (identifier)",
      "lowestGrade": "String",
      "phone": "String",
      "principalEmail": "String",
      "principalName": "String",
      "schoolNumber": "String"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


