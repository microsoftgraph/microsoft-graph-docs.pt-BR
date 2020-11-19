---
title: Atualizar accessReviewScheduleDefinition
description: Atualize um objeto accessReviewScheduleDefinition existente para alterar uma ou mais de suas propriedades.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 06b69bb9e6defcbadb4694d4042fa3bb690ee0f4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221776"
---
# <a name="update-accessreviewscheduledefinition"></a>Atualizar accessReviewScheduleDefinition

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize um objeto [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) existente para alterar uma ou mais de suas propriedades.

>[!NOTE]
>Todas as atualizações feitas em um accessReviewScheduleDefinition se aplicam apenas às instâncias futuras. As instâncias em execução no momento não podem ser atualizadas.
>Além disso, essa API não se destina a atualizar propriedades, incluindo decisões, no nível accessReviewInstance. Consulte [accessReviewInstance](../resources/accessreviewinstance.md) para obter mais informações sobre instâncias.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante)     | AccessReview.ReadWrite.All |
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application                            | AccessReview.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Descrição |
|:-------------|:------------|
|Autorização|{token} de portador. Obrigatório.|
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON de um objeto [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .

A tabela a seguir mostra as propriedades aceitas para atualizar um accessReviewScheduleDefinition.

| Propriedade | Tipo | Descrição |
|:-------------|:------------|:------------|
| displayName | String | Nome da série de revisão do Access. |
| descriptionForAdmins | String | Contexto da revisão fornecida aos administradores. |
| descriptionForReviewers | String | Contexto da revisão fornecida aos revisores. |
| settings | [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md) | As configurações para uma série de análise do Access. Consulte [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md). |
| revisores | coleção [accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|  Define quem é os revisores. Se nenhum for especificado, a revisão será uma autorevisão (os usuários revisaram revisar seu próprio acesso). A propriedade reviewers só será atualizável se os usuários individuais atribuídos forem como revisores. Consulte [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md). | 

Observe que uma solicitação PUT espera que o objeto completo seja passado, no qual todas as propriedades graváveis são incluídas, e não apenas as propriedades que estão sendo atualizadas.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `204, Accepted` código de resposta e nenhum corpo de resposta.

## <a name="examples"></a>Exemplos

Este é um exemplo de atualização do displayName de uma série de análise do Access existente.

### <a name="request"></a>Solicitação
No corpo da solicitação, forneça uma representação JSON das novas propriedades do objeto [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) .



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewScheduleDefinition"
}-->
```http
PUT https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6

{
  "id": "60860cdd-fb4d-4054-91ba-f75e04444aa6",
  "displayName": "Test world UPDATED NAME!",
  "descriptionForAdmins": "Test world",
  "descriptionForReviewers": "Test world",
  "scope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "instanceEnumerationScope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 3,
    "autoApplyDecisionsEnabled": false,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-09-15"
      }
    }
  }
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a>Resposta
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 Accepted
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
