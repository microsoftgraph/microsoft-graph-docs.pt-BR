---
title: Obter accessReviewScheduleDefinition
description: Leia as propriedades e as relações de um objeto accessReviewScheduleDefinition.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 344553abae352f962187068e3b680750762d2579
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979749"
---
# <a name="get-accessreviewscheduledefinition"></a>Obter accessReviewScheduleDefinition
Namespace: microsoft.graph

Leia as propriedades e as relações de [um objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)

Para recuperar as instâncias da série de revisão de acesso, use a API [accessReviewInstance de](accessreviewinstance-list.md) lista.   

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|AccessReview.Read.All, AccessReview.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|AccessReview.Read.All, AccessReview.ReadWrite.All|

Para chamar essa API, o usuário de entrada também deve estar em uma função de diretório que permita que ele leia uma revisão de acesso, ou o usuário pode ser atribuído como revistor na revisão de acesso.  Para obter mais detalhes, consulte os requisitos de função e permissão para [avaliações de acesso.](../resources/accessreviewsv2-root.md)

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewscheduledefinition"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/3856fd6f-36e2-4152-97c9-76070d19f730
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-accessreviewscheduledefinition-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "d6bf2f6c-2f6c-d6bf-6c2f-bfd66c2fbfd6",
    "displayName": "Review example",
    "status": "Applying",
    "scope": {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/v1.0/groups/4444d821-ca3b-45cc-98ee-54c00a04deef/transitiveMembers/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
    },
    "reviewers": [
        {
            "query": "/v1.0/users/5555556e-fce3-4e2d-b28e-4ac0c7d2fa10",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "fallbackReviewers": [],
    "instanceEnumerationScope": {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/v1.0/groups/4444d821-ca3b-45cc-98ee-54c00a04deef",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
    },
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": false,
        "defaultDecisionEnabled": true,
        "defaultDecision": "Deny",
        "instanceDurationInDays": 10,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-04-28",
                "endDate": "2021-05-08"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.disableAndDeleteUserApplyAction"
            }
        ]
    }
  }
}
```

## <a name="see-also"></a>Confira também

- [Criar accessReviewScheduleDefinition](accessreviewscheduledefinition-post.md)
- [Listar accessReviewScheduleDefinition](accessreviewscheduledefinition-list.md)
- [Listar accessReviewInstance](accessreviewinstance-list.md)
