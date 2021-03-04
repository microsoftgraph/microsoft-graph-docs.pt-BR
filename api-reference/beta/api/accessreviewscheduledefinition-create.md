---
title: Criar accessReviewScheduleDefinition
description: Crie um novo objeto accessReviewScheduleDefinition.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b82980e053a50b7562cf94d0a5224badfd1d2a8a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439097"
---
# <a name="create-accessreviewscheduledefinition"></a>Criar accessReviewScheduleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.ReadWrite.All  |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo                            | AccessReview.ReadWrite.All |

O usuário interno também deve estar em uma função de diretório que permita que ele crie uma revisão de acesso.  Para obter mais detalhes, consulte os requisitos de função e permissão para [avaliações de acesso.](../resources/accessreviewsv2-root.md)

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Descrição |
|:-------------|:------------|
|Autorização|{token} de portador. Obrigatório.|
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de um [objeto accessReview.](../resources/accessreview.md)

A tabela a seguir mostra as propriedades aceitas para criar um accessReview.

| Propriedade | Tipo | Descrição |
|:-------------|:------------|:------------|
| displayName | String | Nome da série de revisão de acesso. Obrigatório.|
| descriptionForAdmins | string | Contexto da revisão fornecida aos administradores. Obrigatório. |
  descriptionForReviewers | string | Contexto da revisão fornecida aos revisadores. Obrigatório. |
| escopo | [accessReviewScope](../resources/accessreviewscope.md) | Define o escopo dos usuários revisados em um grupo. Consulte  [accessReviewScope](../resources/accessreviewscheduledefinition.md). Obrigatório.| 
| instanceEnumerationScope | [accessReviewScope](../resources/accessreviewscope.md) | No caso de uma revisão de todos os grupos, isso determina o escopo de quais grupos serão revisados. Consulte [accessReviewScope](../resources/accessreviewscheduledefinition.md). | 
| settings | [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| As configurações de uma série de revisão de acesso. A recorrência é determinada aqui. Consulte [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md). |
| revisadores | [Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) | Define quem são os revisadores. Se nenhum for especificado, a revisão será uma autoavaliação (os usuários revisados analisam seu próprio acesso). Consulte [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md). |


## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201, Created` [objeto accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

Este é um exemplo de criação de uma série de revisão de acesso com um usuário específico, cuja id de objeto de usuário é 7eae4444-d425-48b2-adf2-3c777f6256f3, como revistor. A revisão revisa todos os membros de um grupo específico, cuja id de objeto de grupo é b7a059cb-038a-4802-8fc9-b9d1ed0c4444. Ela se recorre semanalmente.

### <a name="request"></a>Solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
  "displayName": "Test create",
  "descriptionForAdmins": "New scheduled access review",
  "descriptionForReviewers": "If you have any questions, contact jerry@contoso.com",
  "scope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0c4444/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [
    {
      "query": "/users/7eae4444-d425-48b2-adf2-3c777f6256f3",
      "queryType": "MicrosoftGraph",
      "queryRoot": "decisions"
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 1,
    "autoApplyDecisionsEnabled": false,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-09-08T12:02:30.667Z"
      }
    }
  }
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "29f2d16e-9ca6-4052-bbfe-802c48944448",
    "displayName": "Test create",
    "createdDateTime": "0001-01-01T00:00:00Z",
    "lastModifiedDateTime": "0001-01-01T00:00:00Z",
    "status": "NotStarted",
    "descriptionForAdmins": "Test create",
    "descriptionForReviewers": "Test create",
    "instanceEnumerationScope": null,
    "createdBy": {
        "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@contoso.com"
    },
    "scope": {
        "query": "/groups/b74444cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [
        {
            "query": "/users/7eae986b-d425-48b2-adf2-3c777f4444f3",
            "queryType": "MicrosoftGraph",
            "queryRoot": "decisions"
        }
    ],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 1,
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
                "type": "noEnd",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2020-09-08",
                "endDate": null
            }
        },
        "applyActions": []
    }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
