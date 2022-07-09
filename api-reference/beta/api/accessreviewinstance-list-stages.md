---
title: Fases da lista
description: Recupere os estágios em uma instância de revisão de acesso de vários estágios.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: c11b989a29fb14c85d3178e097abd7d82d55f271
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697523"
---
# <a name="list-stages"></a>Fases da lista
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Recupere os estágios em uma instância de revisão de acesso de vários estágios.

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
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stages
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Esse método dá suporte aos `$select`parâmetros de consulta , `$orderby`e `$filter` (`eq` somente) OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de [objetos accessReviewStage](../resources/accessreviewstage.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessreviewstage"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/16d424f6-0100-4bf1-9ebc-fe009c5e5006/instances/bb14c722-51b8-4962-9bd2-1d96ba773d80/stages
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewstage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewstage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewstage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewstage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-accessreviewstage-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewStage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('16d424f6-0100-4bf1-9ebc-fe009c5e5006')/instances('bb14c722-51b8-4962-9bd2-1d96ba773d80')/stages",
    "@odata.count": 2,
    "value": [
        {
            "id": "9ac05ca6-396a-469c-8a8b-bcb98fceb2dd",
            "startDateTime": "2018-08-03T21:02:30.667Z",
            "endDateTime": "2018-08-13T21:17:30.513Z",
            "status": "Completed",
            "reviewers": [
                {
                    "query": "/groups/46d30af1-e626-4928-83f5-e9bfa400289e/owners?$filter=microsoft.graph.user/userType eq 'Member' and microsoft.graph.user/country eq
                    'USA'",
                    "type": "MicrosoftGraph"
                }
            ]
        },
        {
            "id": "03266a48-8731-4cfc-8a60-b2fa6648a14c",
            "startDateTime": "2018-08-14T21:02:30.667Z",
            "endDateTime": "2018-09-03T21:17:30.513Z",
            "status": "InProgress",
            "reviewers": [
                {
                    "queryType": "MicrosoftGraph",
                    "queryRoot": "decisions",
                    "query": "./manager",
                }
            ]
        }
    ]
}
```

