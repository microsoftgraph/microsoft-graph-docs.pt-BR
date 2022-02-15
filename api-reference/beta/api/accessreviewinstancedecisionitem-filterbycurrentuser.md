---
title: 'accessReviewInstanceDecisionItem: filterByCurrentUser'
description: Recupere todos os itens de decisão em uma instância de uma revisão de acesso ou em um estágio de uma instância de uma revisão de acesso em vários estágios, para a qual o usuário de chamada é o revistor.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c2424715661b20dd7fef4efe9291b5efa90c64eb
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2022
ms.locfileid: "62815878"
---
# <a name="accessreviewinstancedecisionitem-filterbycurrentuser"></a>accessReviewInstanceDecisionItem: filterByCurrentUser
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere todos os itens de decisão em uma instância de uma revisão de acesso ou em um estágio de uma instância de uma revisão de acesso em vários estágios, para a qual o usuário de chamada é o revistor. Os itens de decisão são apresentados por um [objeto accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) em um [determinado accessReviewInstance](../resources/accessreviewinstance.md) ou [accessReviewStage](../resources/accessReviewStage.md) para o qual o usuário de chamada é o revisor.


>[!NOTE]
>O tamanho padrão da página para essa API é de 100 **objetos accessReviewInstanceDecisionItem** . Para melhorar a eficiência e evitar tempos-de-tempo devido a grandes conjuntos de resultados, aplique paginação usando os `$skip` parâmetros e `$top` de consulta. Para mais informações, consulte [Paginação de dados do Microsoft Graph em seu aplicativo](/graph/paging).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|AccessReview.Read.All, AccessReview.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|AccessReview.Read.All, AccessReview.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

Para recuperar decisões de uma instância de uma revisão de acesso para a qual o usuário de chamada é o revistor:
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/filterByCurrentUser(on='reviewer')
```

Para recuperar decisões de um estágio em uma instância de uma revisão de acesso para a qual o usuário de chamada é o revistor:
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stages/{accessReviewStageId}/decisions/filterByCurrentUser(on='reviewer')
```

>[!NOTE]
>Os [revisores](../resources/accessreviewschedulesettings.md) de análises em vários estágios podem recuperar as decisões de estágios anteriores se a propriedade **decisionHistoriesForReviewersEnabled** estiver habilitada nas configurações do [objeto accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md).

## <a name="function-parameters"></a>Parâmetros de função
A tabela a seguir mostra os parâmetros de consulta que podem ser usados com esse método.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|on|accessReviewInstanceDecisionItemFilterByCurrentUserOptions|Filtre os objetos de decisão de consulta para o usuário atual. Os valores possíveis são `reviewer`, `unknownFutureValue`. Use `reviewer`. Obrigatório.|


## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte aos `$select`parâmetros de consulta , `$filter``$orderBy`, , `$skip`e `$top` OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma [coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-retrieve-all-decisions-on-an-accessreviewinstance-for-which-the-calling-user-is-the-reviewer"></a>Exemplo 1: Recuperar todas as decisões em um accessReviewInstance para o qual o usuário de chamada é o revisor

#### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstancedecisionitem_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/0185aab8-9a7e-44b5-ae36-41b923c3bf87/instances/1234aab8-9a7e-5678-ae36-41b923c3bf87/decisions/filterByCurrentUser(on='reviewer')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstancedecisionitem-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstancedecisionitem-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstancedecisionitem-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstancedecisionitem-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/accessreviewinstancedecisionitem-filterbycurrentuser-go-snippets.md)]
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(accessReviewInstanceDecisionItem)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
            "id": "139166ec-d214-4835-95aa-3c1d89581e51",
            "accessReviewId": "8d035c9d-798d-47fa-beb4-f986a4b8126f",
            "reviewedDateTime": "2021-05-03T19:28:25.02Z",
            "decision": "Approve",
            "justification": "Christie still needs access to the Marketing group as she works in the Marketing organization.",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "principalLink": "https://graph.microsoft.com/v1.0/users/1800bb2c-955d-4205-8471-3a6c3116435d",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "36c4c56e-fce3-4e2d-b28e-4ac0c7d2fa10",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "1800bb2c-955d-4205-8471-3a6c3116435d",
                "userDisplayName": "Christie Cline",
                "userPrincipalName": "ChristieC@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "1800bb2c-955d-4205-8471-3a6c3116435d",
                "displayName": "Christie Cline",
                "userPrincipalName": "ChristieC@contoso.com"
            }
        }
    ]
}
```

### <a name="example-2-retrieve-all-decisions-on-an-accessreviewstage-of-a-multi-stage-access-review-for-which-the-calling-user-is-the-reviewer"></a>Exemplo 2: Recuperar todas as decisões em um accessReviewStage de uma revisão de acesso em vários estágios para a qual o usuário de chamada é o revisor

#### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "accessreviewinstancedecisionitem_filterbycurrentuser_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/0185aab8-9a7e-44b5-ae36-41b923c3bf87/instances/1234aab8-9a7e-5678-ae36-41b923c3bf87/stages/9458f255-dff2-4d86-9a05-69438f49d7f8/decisions/filterByCurrentUser(on='reviewer')
```

### <a name="response"></a>Resposta
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(accessReviewInstanceDecisionItem)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
            "id": "139166ec-d214-4835-95aa-3c1d89581e51",
            "accessReviewId": "8d035c9d-798d-47fa-beb4-f986a4b8126f",
            "reviewedDateTime": "2021-05-03T19:28:25.02Z",
            "decision": "Approve",
            "justification": "Christie still needs access to the Marketing group as she works in the Marketing organization.",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "principalLink": "https://graph.microsoft.com/v1.0/users/1800bb2c-955d-4205-8471-3a6c3116435d",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "36c4c56e-fce3-4e2d-b28e-4ac0c7d2fa10",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "1800bb2c-955d-4205-8471-3a6c3116435d",
                "userDisplayName": "Christie Cline",
                "userPrincipalName": "ChristieC@contoso.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "1800bb2c-955d-4205-8471-3a6c3116435d",
                "displayName": "Christie Cline",
                "userPrincipalName": "ChristieC@contoso.com"
            }
        }
    ]
}
```
