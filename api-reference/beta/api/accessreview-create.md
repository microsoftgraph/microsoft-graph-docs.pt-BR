---
title: Criar accessReview
description: No recurso de análises de acesso do Azure AD, crie um novo objeto accessReview.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d53f0335ed9b130be65611d049645aba6a7abe44
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439405"
---
# <a name="create-accessreview"></a>Criar accessReview

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de análises de acesso do Azure [AD,](../resources/accessreviews-root.md) crie um novo [objeto accessReview.](../resources/accessreview.md)

Antes de fazer essa solicitação, o chamador deve ter recuperado anteriormente a lista de modelos de fluxo de [negócios,](businessflowtemplate-list.md)para ter o valor de incluir `businessFlowTemplateId` na solicitação.

Depois de fazer essa solicitação, o chamador deve [criar um programControl](programcontrol-create.md), para vincular a revisão de acesso a um programa.  

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | AccessReview.ReadWrite.Membership |

O chamador também deve ter permissão ProgramControl.ReadWrite.All, para que depois de criar uma revisão de acesso, o chamador possa criar um [programControl](../resources/programcontrol.md).
Além disso, o usuário inscreveu também deve estar em uma função de diretório que permita que ele crie uma revisão de acesso.  Para obter mais detalhes, consulte os requisitos de função e permissão para [avaliações de acesso.](../resources/accessreviews-root.md)

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Descrição |
|:-------------|:------------|
| Autorização | \{token\} de portador. Obrigatório. |
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON de um [objeto accessReview.](../resources/accessreview.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar um accessReview.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | O nome da revisão de acesso.  |
| `startDateTime`           |`DateTimeOffset`                                                | DateTime quando a revisão está agendada para ser inicial.  Essa deve ser uma data no futuro.   |
| `endDateTime`             |`DateTimeOffset`                                                | DateTime quando a revisão está agendada para terminar. Isso deve ser pelo menos um dia depois da data de início.   |
| `description`             |`String`                                                        | A descrição, para mostrar aos revisadores. |
| `businessFlowTemplateId`  |`String`                                                        | O identificador do modelo de fluxo de negócios, obtido de um [businessFlowTemplate](../resources/businessflowtemplate.md).  |
| `reviewerType`            |`String`                                                        | O tipo de relação do revistor para os direitos de acesso do objeto revisado, um `self` de `delegated` , ou `entityOwners` . | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | O objeto para o qual uma revisão de acesso é criada, como a associação de um grupo ou as atribuições de usuários a um aplicativo. | 


Se o reviewerType fornecido tiver o valor , o chamador também deverá incluir a propriedade, com uma coleção de `delegated` `reviewers` [userIdentity](../resources/useridentity.md) dos revisadores.

Se seu aplicativo estiver chamando essa API sem um usuário ligado, o chamador também deverá incluir a propriedade **createdBy,** o valor para o qual é uma [userIdentity](../resources/useridentity.md) do usuário que será identificado como o criador da revisão.

Além disso, o chamador pode incluir configurações, para criar uma série de revisão recorrente ou para alterar do comportamento de revisão padrão. Em particular, para criar uma revisão recorrente, o chamador deve incluir as configurações de revisão `accessReviewRecurrenceSettings` de acesso,


## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201, Created` [objeto accessReview](../resources/accessreview.md) no corpo da resposta.

## <a name="example"></a>Exemplo

Este é um exemplo de criação de uma revisão de acesso única (não recorrente), especificando explicitamente dois usuários como revistores.

### <a name="request"></a>Solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto accessReview.](../resources/accessreview.md)

<!-- {
  "blockType": "ignored",
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
        "id": "99025615-a0b1-47ec-9117-35377b10998b"
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

### <a name="response"></a>Resposta
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
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
  ]
}
-->


