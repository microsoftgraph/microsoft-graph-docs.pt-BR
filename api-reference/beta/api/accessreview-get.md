---
title: Obter accessReview
description: 'No Windows Azure AD para acessar o recurso de revisões, recuperar um objeto accessReview.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 26551f27fdf328865509cd02011f3ee2344f5e82
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529142"
---
# <a name="get-accessreview"></a>Obter accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de [acesso analisa](../resources/accessreviews-root.md) Azure AD, recupere um objeto de [accessReview](../resources/accessreview.md) .  

Para recuperar os revisores da revisão access, use os [Revisores de accessReview lista](accessreview-listreviewers.md) API. Para recuperar as decisões da revisão access, use a API de [decisões de accessReview de lista](accessreview-listdecisions.md) ou a API de [Listar Minhas decisões accessReview](accessreview-listmydecisions.md) .

Se essa for uma análise mais acesso recorrente, em seguida, use o `instances` relação para recuperar uma coleção de [accessReview](../resources/accessreview.md) de passado, instâncias atuais e futuros da revisão acesso.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | `AccessReview.Read.All`, `AccessReview.ReadWrite.All`.  O usuário conectado também deve ser em uma função de diretório que permite que uma revisão de acesso de leitura ou atribuído como um revisor na revisão de acesso. |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | Token de portador Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Nenhum corpo da solicitação deve ser fornecido.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200, OK` código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')
```

##### <a name="response"></a>Resposta
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
    "displayName": "review",
    "startDateTime": "2017-11-14T01:14:54.89Z",
    "endDateTime": "2017-12-14T01:14:54.89Z",
    "status": "InProgress",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "self",
    "description": "",
    "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"},
    "settings": {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval": true,
        "autoReviewEnabled": false,
        "activityDurationInDays": 30,
        "autoApplyReviewResultsEnabled": false,
        "accessRecommendationsEnabled": false,
        "recurrenceSettings": {
            "recurrenceType": "onetime",
            "recurrenceEndType": "endBy",
            "durationInDays": 0,
            "recurrenceCount": 0
        },
        "autoReviewSettings": {
            "notReviewedResult": "Deny"
        }
    }
}
```

## <a name="see-also"></a>Confira também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar accessReview](accessreview-create.md) |    [accessReview](../resources/accessreview.md) |  Crie um novo accessReview. |
|[Lista programControls](programcontrol-list.md) | coleção [programControl](../resources/programcontrol.md) | Listar programControls em um locatário. |
|[Listar accessReview revisores](accessreview-listreviewers.md) |     coleção [userIdentity](../resources/useridentity.md)|    Obtenha os revisores de um accessReview. |
|[Lista accessReview decisões](accessreview-listdecisions.md) |     coleção [accessReviewDecision](../resources/accessreviewdecision.md)|    Obtenha as decisões de um accessReview.|
|[Listar meus decisões accessReview](accessreview-listmydecisions.md) |        coleção [accessReviewDecision](../resources/accessreviewdecision.md)|    Como um revisor, obtenha Minhas decisões de um accessReview.|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
