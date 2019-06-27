---
title: Listar minhas decisões do accessReview
description: No recurso de revisões do Azure AD Access, recupere as decisões de um objeto accessReview para o usuário de chamada como revisor.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6b506ab17abe270bfd3ecc27ab70f7699487528a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258846"
---
# <a name="list-my-accessreview-decisions"></a>Listar minhas decisões do accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere as decisões de um objeto [accessReview](../resources/accessreview.md) para o usuário de chamada como revisor.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview. Read. All, AccessReview. ReadWrite. All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |

O usuário conectado também deve ter permissão para ler essa revisão de acesso específica.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/myDecisions
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Nenhum corpo de solicitação deve ser fornecido.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um `200, OK` código de resposta e uma matriz de objetos [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta, para o qual o usuário de chamada é um revisor atribuído.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions
```

##### <a name="response"></a>Resposta
>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewDecision",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
            "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "accessReviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "reviewResult": "Approve",
            "userPrincipalName": "alice@litware.com",
            "userId": "Alice Smith"
    }
    ]
}
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_accessReview_decisions-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="see-also"></a>Confira também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter accessReview](accessreview-get.md) |  [accessReview](../resources/accessreview.md) |  Recupere uma revisão do Access. |
|[Listar decisões accessReview](accessreview-listdecisions.md) |     coleção [accessReviewDecision](../resources/accessreviewdecision.md)|    Recuperar todas as decisões de um accessReview.|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/accessreview-listmydecisions.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
