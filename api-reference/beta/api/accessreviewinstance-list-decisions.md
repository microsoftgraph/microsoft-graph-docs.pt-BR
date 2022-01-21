---
title: Listar decisões
description: Obter os recursos accessReviewInstanceDecisionItem da propriedade de navegação de decisões.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 138d53b3d0c497601b0bdfe50512ca71ddfd68d9
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/21/2022
ms.locfileid: "62161813"
---
# <a name="list-decisions"></a>Listar decisões
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere os [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) para um [accessReviewInstance específico.](../resources/accessreviewinstance.md) Uma lista de zero ou mais objetos accessReviewInstanceDecisionItem é retornada, incluindo todas as suas propriedades aninhadas.

>[!NOTE]
>O tamanho padrão da página para essa API é de 100 objetos accessReviewInstance. Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta. Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|AccessReview.Read.All, AccessReview.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|AccessReview.Read.All, AccessReview.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte a parâmetros de consulta `$select` , , , e `$filter` `$orderBy` `$skip` `$top` OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-retrieve-all-decisions-for-an-instance-of-an-access-review"></a>Exemplo 1: recuperar todas as decisões de uma instância de uma revisão de acesso

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-444404f3baa6/instances/14444cdb-6a18-4c08-ba2c-48c02f0a0138/decisions?$top=100&$skip=0
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-accessreviewinstancedecisionitem-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewInstanceDecisionItem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0')/instances('6444d4fd-ab55-4608-8cf9-c6702d172bcc')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "e6cafba0-cbf0-4748-8868-0810c7f4cc06",
            "accessReviewId": "6444d4fd-ab55-4608-8cf9-c6702d172bcc",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
                "userDisplayName": "Diego Siciliani",
                "userPrincipalName": "DiegoS@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
                "displayName": "Diego Siciliani",
                "userPrincipalName": "DiegoS@contoso.com"
            }
        },
        {
            "id": "4bde8d40-9224-4aa3-936b-08d73e1baf47",
            "accessReviewId": "6444d4fd-ab55-4608-8cf9-c6702d172bcc",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/11feb738-0039-4a6c-a045-dcb91a47969a",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "11feb738-0039-4a6c-a045-dcb91a47969a",
                "userDisplayName": "Johanna Lorenz",
                "userPrincipalName": "JohannaL@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "11feb738-0039-4a6c-a045-dcb91a47969a",
                "displayName": "Johanna Lorenz",
                "userPrincipalName": "JohannaL@contoso.com"
            }
        }
    ]
}
```


### <a name="example-2-retrieve-all-decision-items-for-which-youre-a-reviewer-and-expand-the-definitions"></a>Exemplo 2: recupere todos os itens de decisão para os quais você é revistor e expanda as definições

#### <a name="request"></a>Solicitação
O exemplo a seguir mostra uma solicitação para recuperar todas as decisões em cada instância e a definição de que o usuário de chamada é o revistor.

<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem_expand"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/decisions/filterByCurrentUser(on='reviewer')?$expand=instance($expand=definition)
```

### <a name="response"></a>Resposta

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#accessReviewInstanceDecisionItems",
    "@odata.count": 10,
    "value": [
        {
            "id": "fa73e90b-5bf1-45fd-a182-35ce5fc0674d",
            "principal": {
                    "odata.type": "#microsoft.graph.userIdentity",
                    "id": "a6c7aecb-cbfd-4763-87ef-e91b4bd509d9",
                    "displayName": "Adele Vance",
                    "userPrincipalName": "adele@contoso.com"            
            },
            "resource": {
                "odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",              
                "id": "b4cbd87c-0ee2-4647-a7e3-41b580ea6fed",
                "displayName": "Priviliged Role Administrator",
                "type": "azureRole",
                "scope": {
                    "id": "b649368b-d667-40c6-acc9-b45b822a3037",
                    "displayName": "Hello world",
                    "type": "subscription"
                }
            },
            "instance": {
                "startDate": "2018-08-03T21:02:30.667Z",
                "endDate": "2018-08-05T21:02:30.667Z",
                "definition": {
                     "displayName": "Hello world",
                     "descriptionForAdmins": "Hello world"
                }
            }
        },
        {
            "id": "fa73e90b-5bf1-45fd-a182-35ce5fc0674d",
            "principal": {
                    "odata.type": "#microsoft.graph.userIdentity",
                    "id": "a6c7aecb-cbfd-4763-87ef-e91b4bd509d9",
                    "displayName": "Adele Vance",
                    "userPrincipalName": "adele@contoso.com"            
            },
            "resource": {
                "odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",              
                "id": "f1edce7a-edad-49fb-83eb-b7f1eda48dd2",
                "displayName": "Global Administrator",
                "type": "azureRole",
                "scope": {
                    "id": "b649368b-d667-40c6-acc9-b45b822a3037",
                    "displayName": "Hello world",
                    "type": "subscription"
                }
            },
            "instance": {
                "startDate": "2018-08-03T21:02:30.667Z",
                "endDate": "2018-08-05T21:02:30.667Z",
                "definition": {
                     "displayName": "Hello world",
                     "descriptionForAdmins": "Hello world"
                }
            }
        },
        {
            "id": "fa73e90b-5bf1-45fd-a182-35ce5fc0674d",
            "principal": {
                    "odata.type": "#microsoft.graph.userIdentity",
                    "id": "a6c7aecb-cbfd-4763-87ef-e91b4bd509d9",
                    "displayName": "John Doe",
                    "userPrincipalName": "johndoe@contoso.com"            
            },
            "resource": {
                "odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",              
                "id": "f1edce7a-edad-49fb-83eb-b7f1eda48dd2",
                "displayName": "Global Administrator",
                "type": "azureRole",
                "scope": {
                    "id": "b649368b-d667-40c6-acc9-b45b822a3037",
                    "displayName": "Hello world",
                    "type": "subscription"
                }
            },
            "instance": {
                "startDate": "2018-08-03T21:02:30.667Z",
                "endDate": "2018-08-05T21:02:30.667Z",
                "definition": {
                     "displayName": "Hello world",
                     "descriptionForAdmins": "Hello world"
                }
            }
        },
        {
            "id": "2e8e717b-a857-49f0-918a-013cf0415456",
            "principal": {
                    "odata.type": "#microsoft.graph.userIdentity",
                    "id": "a6c7aecb-cbfd-4763-87ef-e91b4bd509d9",
                    "displayName": "John Doe 1",
                    "userPrincipalName": "johndoe1@contoso.com"            
            },
            "resource": {
                "odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemAzureRoleResource",              
                "id": "20a97808-56dd-490a-97a9-73bf2344cce7",
                "displayName": "Hello world",
                "type": "azureRole",
                "scope": {
                    "id": "b649368b-d667-40c6-acc9-b45b822a3037",
                    "displayName": "Hello world",
                    "type": "subscription"
                }
            },
            "instance": {
                "startDate": "2018-08-03T21:02:30.667Z",
                "endDate": "2018-08-05T21:02:30.667Z",
                "definition": {
                     "displayName": "Hello world",
                     "descriptionForAdmins": "Hello world"
                }
            }
        }
    ]
}
```
