---
title: Obter accessReviewInstanceDecisionItem
description: Leia as propriedades e as relações de um objeto accessReviewInstanceDecisionItem.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f245e99cc6b10b5acb2ea44037e158fcd97afd6a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987702"
---
# <a name="get-accessreviewinstancedecisionitem"></a>Obter accessReviewInstanceDecisionItem
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Leia as propriedades e as relações de um [objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|AccessReview.Read.All, AccessReview.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|AccessReview.Read.All, AccessReview.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método dá suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/decisions/e6cafba0-cbf0-4748-8868-0810c7f4cc06
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-accessreviewinstancedecisionitem-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0')/instances('6444d4fd-ab55-4608-8cf9-c6702d172bcc')/decisions/$entity",
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
}
```
