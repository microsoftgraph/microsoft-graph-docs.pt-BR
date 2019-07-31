---
title: Criar accessReview
description: No recurso de revisões do Azure AD Access, crie um novo objeto accessReview.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ab1711a370d766631611d9cd5f96635760f98f48
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35946052"
---
# <a name="create-accessreview"></a>Criar accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , crie um novo objeto [accessReview](../resources/accessreview.md) .

Antes de fazer essa solicitação, o chamador deve ter [recuperado previamente a lista de modelos de fluxo de negócios](businessflowtemplate-list.md), para que `businessFlowTemplateId` o valor de seja incluído na solicitação.

Depois de fazer essa solicitação, o chamador deve [criar um programControl](programcontrol-create.md)para vincular a revisão do Access a um programa.  

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |

O chamador também deve ter a permissão ProgramControl. ReadWrite. All, de modo que depois de criar uma revisão do Access, o chamador possa criar um [ProgramControl](../resources/programcontrol.md).
Além disso, o usuário conectado também deve estar em uma função de diretório que permite que eles criem uma revisão do Access.  Para obter mais detalhes, consulte a função e os requisitos de permissão para [revisões do Access](../resources/accessreviews-root.md).

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON de um objeto [accessReview](../resources/accessreview.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar um accessReview.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | O nome de revisão do acesso.  |
| `startDateTime`           |`DateTimeOffset`                                                | O DateTime quando a revisão está agendada para ser iniciada.  Isso deve ser uma data no futuro.   |
| `endDateTime`             |`DateTimeOffset`                                                | O DateTime quando a revisão é agendada para terminar. Este deve ser pelo menos um dia depois da data de início.   |
| `description`             |`String`                                                        | A descrição, para mostrar aos revisores. |
| `businessFlowTemplateId`  |`String`                                                        | O identificador do modelo de fluxo de negócios obtido de um [businessFlowTemplate](../resources/businessflowtemplate.md).  |
| `reviewerType`            |`String`                                                        | O tipo de relação de revisor para os direitos de acesso do objeto revisado, `self`um `delegated`de, `entityOwners`ou. | 
| `reviewedEntity`          |`microsoft.graph.identity`                                      | O objeto para o qual uma revisão de acesso é criada, como a associação de um grupo ou as atribuições de usuários a um aplicativo. | 


Se o revisortype que está sendo fornecido tiver `delegated`o valor, o chamador também deverá incluir `reviewers` a propriedade, com uma coleção de UserIdentity dos revisores. [](../resources/useridentity.md)

Se seu aplicativo estiver chamando esta API sem um usuário conectado, o chamador também deverá incluir a propriedade **createdBy** , o valor para o qual é um UserIdentity [](../resources/useridentity.md) do usuário que será identificado como criador da revisão.

Além disso, o chamador pode incluir configurações, para criar uma série de análise recorrente ou para alterar o comportamento de revisão padrão. Em particular, para criar uma revisão recorrente, o chamador deve incluir as `accessReviewRecurrenceSettings` configurações de revisão do Access,


## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201, Created` um código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.

## <a name="example"></a>Exemplo

Este é um exemplo de criação de uma revisão de acesso de uma única vez (não recorrente), especificando explicitamente dois usuários como os revisores.

##### <a name="request"></a>Solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [accessReview](../resources/accessreview.md) .


# <a name="httptabhttp"></a>[HTTP](#tab/http)
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
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreview-from-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreview-from-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objetivo-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreview-from-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreview-from-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta
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
