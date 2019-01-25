---
title: Criar accessReview
description: No Windows Azure AD para acessar o recurso de revisões, crie um novo objeto accessReview.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 669b11a8f3b52e867d6b3e803c9419968924928b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517796"
---
# <a name="create-accessreview"></a>Criar accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, cria um novo objeto [accessReview](../resources/accessreview.md) .

Antes de fazer essa solicitação, o chamador deve ter anteriormente [recuperada a lista de modelos de fluxo de negócios](businessflowtemplate-list.md), para que o valor de `businessFlowTemplateId` para incluir na solicitação.

Depois de fazer essa solicitação, o chamador deve [criar um programControl](programcontrol-create.md), para vincular a revisão de acesso a um programa.  

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.ReadWrite.All e também devem ter ProgramControl.ReadWrite.All ao cenário completo com a chamada subsequente para criar um programControl |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | Token de portador Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de um objeto [accessReview](../resources/accessreview.md) .

A tabela a seguir mostra as propriedades que são necessárias quando você cria um accessReview.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | O nome de revisão de acesso.  |
| `startDateTime`           |`DateTimeOffset`                                                | DateTime quando a revisão está agendada para ser iniciar.  Isso deve ser uma data no futuro.   |
| `endDateTime`             |`DateTimeOffset`                                                | DateTime quando a revisão está agendada para terminar. Isto deve ser de pelo menos um dia mais recente do que a data de início.   |
| `description`             |`String`                                                        | A descrição, para mostrar aos revisores. |
| `businessFlowTemplateId`  |`String`                                                        | O identificador de modelo de fluxo corporativos, obtido de uma [businessFlowTemplate](../resources/businessflowtemplate.md).  |
| `reviewerType`            |`String`                                                        | O tipo de relacionamento de revisor para os direitos de acesso do objeto revisado, uma das `self`, `delegated`, ou `entityOwners`. | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | O objeto para o qual uma revisão de acesso é criada, como a associação de um grupo ou as atribuições de usuários para um aplicativo. | 


Se o reviewerType sendo fornecido tem o valor `delegated`, e em seguida, o chamador também deverá incluir o `reviewers` propriedade, com uma coleção de [userIdentity](../resources/useridentity.md) dos revisores.

Além disso, o chamador pode incluir configurações, para criar uma série recorrente de revisão ou alterar do comportamento padrão de revisão. Em particular, para criar uma análise mais recorrente, o chamador deve incluir a `accessReviewRecurrenceSettings` dentro do access, revise as configurações,


## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201, Created` código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.

## <a name="example"></a>Exemplo

Este é um exemplo de criação de uma única (não recorrente) de revisão de acesso, especificando explicitamente os dois usuários como revisores.

##### <a name="request"></a>Solicitação
No corpo da solicitação, fornece uma representação JSON do objeto [accessReview](../resources/accessreview.md) .

<!-- {
  "blockType": "request",
  "name": "create_accessReview_from_accessReviews"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews
Content-type: application/json

{
    "displayName":"TestReview",
    "startDateTime":"2017-02-10T00:35:53.214Z",
    "endDateTime":"2017-03-12T00:35:53.214Z",
    "reviewedEntity": {
        "id": "99025615-a0b1-47ec-9117-35377b10998b",
    },
    "reviewerType" : "delegated",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "description":"Sample description",
    "reviewers":
    [
        {
            "id":"f260246a-09b1-4fd5-8d18-daed736071ec"
        },
        {
            "id":"5a4e184c-4ee5-4883-96e9-b371f8da88e3"
        }
    ],
    "settings":
    {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval":true,
        "autoReviewEnabled":false,
        "activityDurationInDays":30,
        "autoApplyReviewResultsEnabled":false,
        "accessRecommendationsEnabled":false,
        "recurrenceSettings":{
            "recurrenceType":"onetime",
            "recurrenceEndType":"endBy",
            "durationInDays":0,
            "recurrenceCount":0
        },
        "autoReviewSettings":{
            "notReviewedResult":"Deny"
        }
    }
}
```

##### <a name="response"></a>Resposta
>**Observação: **o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview",
    "startDateTime": "2017-02-10T00:35:53.214Z",
    "endDateTime": "2017-03-12T00:35:53.214Z",
    "status": "Initializing",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "delegated",
    "description": "Sample description"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "Create accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
