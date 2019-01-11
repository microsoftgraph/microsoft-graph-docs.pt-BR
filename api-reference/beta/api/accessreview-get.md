---
title: Obter accessReview
description: 'No Windows Azure AD para acessar o recurso de revisões, recuperar um objeto accessReview.  '
localization_priority: Normal
ms.openlocfilehash: 471cebe3dbfa60e6cc05e2be546504216163ee0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894037"
---
# <a name="get-accessreview"></a>Obter accessReview

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

No recurso de [acesso analisa](../resources/accessreviews-root.md) Azure AD, recupere um objeto de [accessReview](../resources/accessreview.md) .  

Para recuperar os revisores da revisão access, use os [Revisores de accessReview lista](accessreview-listreviewers.md) API. Para recuperar as decisões da revisão access, use a API de [decisões de accessReview de lista](accessreview-listdecisions.md) ou a API de [Listar Minhas decisões accessReview](accessreview-listmydecisions.md) .

Se essa for uma análise mais acesso recorrente, em seguida, use o `instances` relação para recuperar uma coleção de [accessReview](../resources/accessreview.md) de passado, instâncias atuais e futuros da revisão acesso.

## <a name="permissions"></a>Permissions
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
| Autorização | string | Portador \{token\}. Obrigatório. |

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
    "settings": {
        "reviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval": true,
        "recurrenceSettings": {
            "recurrenceType": "onetime",
            "recurrenceEndType": "endBy",
            "durationInDays": 0,
            "recurrenceCount": 0
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


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
