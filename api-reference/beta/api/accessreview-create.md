---
title: Criar accessReview
description: No recurso de análises de acesso do Azure AD, crie um novo objeto accessReview.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 516a1567921089f1285d639f4e12f8747e92de91
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988151"
---
# <a name="create-accessreview"></a>Criar accessReview

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de análises de acesso do Azure [AD,](../resources/accessreviews-root.md) crie um novo [objeto accessReview.](../resources/accessreview.md)

Antes de fazer essa solicitação, o chamador deve ter recuperado anteriormente a lista de modelos de fluxo de negócios [,](businessflowtemplate-list.md)para ter o valor **de businessFlowTemplateId** para incluir na solicitação.

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
| displayName             |Cadeia de caracteres                                                        | O nome da revisão de acesso.  |
| startDateTime           |DateTimeOffset                                                | DateTime quando a revisão está agendada para ser inicial.  Essa deve ser uma data no futuro.   |
| endDateTime             |DateTimeOffset                                                | DateTime quando a revisão está agendada para terminar. Isso deve ser pelo menos um dia depois da data de início.   |
| description             |String                                                        | A descrição, para mostrar aos revisadores. |
| businessFlowTemplateId  |Cadeia de caracteres                                                        | O identificador do modelo de fluxo de negócios, obtido de um [businessFlowTemplate](../resources/businessflowtemplate.md).  |
| reviewerType            |Cadeia de caracteres                                                        | O tipo de relação do revistor para os direitos de acesso do objeto revisado, um `self` de `delegated` , ou `entityOwners` . | 
| reviewedEntity          |[identity](../resources/identity.md)                                     | O objeto para o qual uma revisão de acesso é criada, como a associação de um grupo ou as atribuições de usuários a um aplicativo. | 


Se o **reviewerType** tiver o valor , o chamador também deverá incluir a propriedade reviewers, com uma coleção de objetos `delegated` [userIdentity](../resources/useridentity.md) representando os revistores. 

Se seu aplicativo estiver chamando essa API sem um usuário ligado, o chamador também deverá incluir a propriedade **createdBy,** o valor para o qual é uma [userIdentity](../resources/useridentity.md) do usuário que será identificado como o criador da revisão.

Além disso, o chamador pode incluir **configurações**, para criar uma série de revisão recorrente ou para alterar do comportamento de revisão padrão. Em particular, para criar uma revisão recorrente, o chamador deve incluir [accessReviewRecurrenceSettings](../resources/accessreviewrecurrencesettings.md) dentro das configurações de revisão de acesso,


## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto accessReview](../resources/accessreview.md) no corpo da resposta.

## <a name="example"></a>Exemplo

Este é um exemplo de criação de uma revisão de acesso única (não recorrente), especificando explicitamente dois usuários como revistores.

### <a name="request"></a>Solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto accessReview.](../resources/accessreview.md)


# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreview-from-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreview-from-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreview-from-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreview-from-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-accessreview-from-accessreviews-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
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


