---
title: Atualizar accessReview
description: No recurso de análises de acesso do Azure AD, atualize um objeto accessReview existente para alterar uma ou mais de suas propriedades.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 6de1862411d20f1e1fc68fc202a5e59aa888f165
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439258"
---
# <a name="update-accessreview"></a>Atualizar accessReview

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de análises de acesso do Azure [AD,](../resources/accessreviews-root.md) atualize um objeto [accessReview](../resources/accessreview.md) existente para alterar uma ou mais de suas propriedades.

Essa API não se destina a alterar os revisadores ou decisões de uma revisão.  Para alterar os revisores, use [as APIs addReviewer](accessreview-addreviewer.md) [ou removeReviewer.](accessreview-removereviewer.md)  Para interromper uma revisão já iniciada uma vez ou uma instância já iniciada de uma revisão recorrente, antes, use a API [stop.](accessreview-stop.md) Para aplicar as decisões ao grupo de destino ou aos direitos de acesso ao aplicativo, use a API [de aplicação.](accessreview-apply.md) 


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | AccessReview.ReadWrite.Membership |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews/{reviewId}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON dos parâmetros de um [objeto accessReview.](../resources/accessreview.md)

A tabela a seguir mostra as propriedades que podem ser fornecidas quando você atualiza um accessReview.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | O nome da revisão de acesso.  |
| `startDateTime`           |`DateTimeOffset`                                                | DateTime quando a revisão está agendada para ser inicial.  Essa deve ser uma data no futuro.   |
| `endDateTime`             |`DateTimeOffset`                                                | DateTime quando a revisão está agendada para terminar. Isso deve ser pelo menos um dia depois da data de início.   |
| `description`             |`String`                                                        | A descrição, para mostrar aos revisadores. |



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `204, Accepted` [objeto accessReview](../resources/accessreview.md) no corpo da resposta.

## <a name="example"></a>Exemplo

Este é um exemplo de atualização de uma revisão de acesso única (não recorrente).

##### <a name="request"></a>Solicitação
No corpo da solicitação, fornece uma representação JSON das novas propriedades do [objeto accessReview.](../resources/accessreview.md)


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews/006111db-0810-4494-a6df-904d368bd81b
Content-type: application/json

{
    "displayName":"TestReview new name"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreview-java-snippets.md)]
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
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "006111db-0810-4494-a6df-904d368bd81b",
    "displayName": "TestReview new name",
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
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


