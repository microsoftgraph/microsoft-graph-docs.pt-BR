---
title: 'accessReviewStage: filterByCurrentUser'
description: Retornar todos os objetos accessReviewStage para um determinado revisor.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f224acfdd86ca07a211a1389125524d90b7b8a07
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816130"
---
# <a name="accessreviewstage-filterbycurrentuser"></a>accessReviewStage: filterByCurrentUser
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Retorne todos os objetos [accessReviewStage](../resources/accessReviewStage.md) em um [determinado accessReviewInstance](../resources/accessreviewinstance.md) onde o usuário de chamada é um revisor em um ou mais objetos [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) .

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
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stages/filterByCurrentUser(on='reviewer')
```

## <a name="function-parameters"></a>Parâmetros de função
Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.
A tabela a seguir mostra os parâmetros que podem ser usados com esta função.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|on|accessReviewStageFilterByCurrentUserOptions|Filtra os resultados com base no usuário de chamada. O valor permitido é `reviewer`. Isso retorna todos os objetos accessReviewStage no accessReviewInstance onde o usuário de chamada é um revisor. Obrigatório.|

Essa função também dá suporte aos `$select`parâmetros de consulta , `$filter`, `$orderBy`e `$skip` `$top` OData para ajudar a personalizar a resposta. Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma [coleção accessReviewStage](../resources/accessreviewstage.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "accessreviewstage_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/08531375-eff6-4e21-b1a8-de0eb37ec913/instances/86889534-b102-4226-bfce-0c2aeee845df/stages/filterByCurrentUser(on='reviewer')
```


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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(accessReviewStage)",
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

