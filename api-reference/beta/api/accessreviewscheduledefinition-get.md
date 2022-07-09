---
title: Obter accessReviewScheduleDefinition
description: Recupere um objeto accessReviewScheduleDefinition.
ms.localizationpriority: medium
author: zhusijia26
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 96ac40ba6b7785e3fa3465d1bbb0a15afb6a0ac1
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66696850"
---
# <a name="get-accessreviewscheduledefinition"></a>Obter accessReviewScheduleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere um [objeto accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) por ID. Isso retorna todas as propriedades da série de revisão de acesso agendada, exceto o accessReviewInstances associado. Cada accessReviewScheduleDefinition tem pelo menos uma instância. Uma instância representa uma revisão de um recurso específico (como membros de um grupo específico), durante uma ocorrência (por exemplo, março de 2021) de uma revisão recorrente.

Para recuperar as instâncias da série de revisão de acesso, use a API [accessReviewInstance de](accessreviewscheduledefinition-list-instances.md) lista.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.Read.All, AccessReview.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo                            | AccessReview.Read.All, AccessReview.ReadWrite.All |

Para chamar essa API, o usuário conectado também deve estar em uma função de diretório que permita ler uma revisão de acesso ou o usuário pode ser atribuído como revistor na revisão de acesso.  Para obter mais detalhes, consulte os requisitos de função e permissão para [revisões de acesso](../resources/accessreviewsv2-overview.md).

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{review-id}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método dá suporte `$select` a parâmetros de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
Nenhum.

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna `200 OK` um código de resposta e um [objeto accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) no corpo da resposta.

## <a name="examples"></a>Exemplos
### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviewScheduleDefinition"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d
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

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-accessreviewscheduledefinition-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "60860cdd-fb4d-4054-91ba-f7544443baa6",
    "displayName": "Test world",
    "status": "InProgress",
    "scope": {
        "query": "/groups/b7a059cb-038a-4802-8fc9-b944440cf11f/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups/b7a059cb-038a-4802-8fc9-b9d14444f11f",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 0,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": {
                "type": "weekly",
                "interval": 1,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2020-09-15",
                "endDate": "9999-12-31"
            }
        }
    }
}
```

## <a name="see-also"></a>Confira também

- [Criar accessReviewScheduleDefinition](accessreviewset-post-definitions.md)
- [Listar accessReviewScheduleDefinition](accessreviewset-list-definitions.md)
- [Listar accessReviewInstance](accessreviewscheduledefinition-list-instances.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
