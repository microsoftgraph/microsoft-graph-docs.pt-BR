---
title: 'accessReviewInstance: pendingAccessReviewInstances'
description: Recupere os objetos accessReviewInstance aguardando aprovação chamando o usuário.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 581ade7ffd620a105dfbb2e6f5c8e9854aab76dc
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048411"
---
# <a name="accessreviewinstance-pendingaccessreviewinstances"></a>accessReviewInstance: pendingAccessReviewInstances

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere os [objetos accessReviewInstance](../resources/accessreviewinstance.md) pendentes aprovação pelo usuário de chamada. Uma lista de zero ou mais objetos accessReviewInstance são retornados, dos quais o usuário de chamada é um revisor atribuído.

>[!NOTE]
>Se muitos **accessReviewInstances são retornados,** para melhorar a eficiência e evitar tempos-extra, recupere o resultado definido em páginas, incluindo o parâmetro de consulta $top com um tamanho de página de no máximo 100 e o parâmetro de consulta $skip=0 na solicitação. Quando um conjunto de resultados abrange várias páginas, o Microsoft Graph retorna essa página com uma propriedade @odata.nextLink na resposta que contém uma URL para a próxima página de resultados. Se essa propriedade estiver presente, continue fazendo solicitações adicionais com a URL @odata.nextLink em cada resposta, até que todos os resultados sejam retornados, conforme descrito na pa paja do Microsoft Graph dados em seu aplicativo.
>
>Se nenhum parâmetro de consulta for fornecido e houver mais de 100 resultados, o Microsoft Graph paginará automaticamente os resultados em 100 resultados por página.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.Read.All, AccessReview.ReadWrite.All  |

 O usuário in-loco só vê instâncias das quais são atribuídas revisores no accessReviewScheduleDefinition da instância.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
Nenhum

## <a name="request-body"></a>Corpo da solicitação
Não fornecer um corpo de solicitação.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e uma matriz de `200 OK` [objetos accessReviewInstance](../resources/accessreviewinstance.md) no corpo da resposta.

## <a name="examples"></a>Exemplos
### <a name="request"></a>Solicitação
O exemplo a seguir mostra uma solicitação para recuperar todas as séries de revisão de acesso em um locatário.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances?$expand=definition&$top=100&$skip=0
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-pendingapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-pendingapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-pendingapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-pendingapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.count": 1,
    "value": [
        {
            "id": "70a68410-67f3-4d4c-b946-6989e050be19",
            "startDateTime": "2020-09-09T15:57:56Z",
            "endDateTime": "2020-10-08T15:57:56Z",
            "status": "InProgress",
            "scope": {
                "query": "/groups/04b3d70b-c770-46cb-b751-d857d2beedff/transitiveMembers",
                "queryType": "MicrosoftGraph"
            },
            "definition": {
                "id": "70a68410-67f3-4d4c-b946-6989e050be19",
                "displayName": "review of leadership",
                "createdDateTime": "2020-09-08T15:59:06Z",
                "lastModifiedDateTime": "2020-09-09T15:58:24Z",
                "status": "InProgress",
                "descriptionForAdmins": "review of leadership",
                "descriptionForReviewers": "",
                "createdBy": {
                    "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@msft.com"
                },
                "scope": {
                    "query": "/groups/04b3d70b-c770-46cb-b751-d857d2beedff/transitiveMembers",
                    "queryType": "MicrosoftGraph"
                },
                "instanceEnumerationScope": {
                    "query": "/groups/04b3d70b-c770-46cb-b751-d857d2beedff",
                    "queryType": "MicrosoftGraph"
                },
                "reviewers": [
                    {
                        "query": "/users/957f1027-c0ee-460d-9269-b8828e59e0fe",
                        "queryType": "MicrosoftGraph",
                        "queryRoot": null
                    }
                ],
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
                        "pattern": null,
                        "range": {
                            "type": "numbered",
                            "numberOfOccurrences": 0,
                            "recurrenceTimeZone": null,
                            "startDate": "2020-09-09",
                            "endDate": "2020-10-08"
                        }
                    },
                    "applyActions": [
                        {
                            "@odata.type": "#microsoft.graph.removeAccessApplyAction"
                        }
                    ]
                }
            }
        }
    ]
}
```

## <a name="see-also"></a>Confira também

- [Obter accessReviewInstance](accessreviewinstance-get.md)
- [Obter a aprovação pendente accessReviewInstanceDecisionItems](accessreviewinstancedecisionitem-listpendingapproval.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstance pendingApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
