---
title: Atualizar accessReview (preterido)
description: No recurso Azure AD de revisões de acesso, atualize um objeto accessReview existente para alterar uma ou mais de suas propriedades.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: eb7bc62b0ca05ff985bfb9a06d776d3ed7a2a2eb
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819126"
---
# <a name="update-accessreview-deprecated"></a>Atualizar accessReview (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

No recurso Azure AD [revisões de acesso](../resources/accessreviews-root.md), atualize um objeto [accessReview](../resources/accessreview.md) existente para alterar uma ou mais de suas propriedades.

Essa API não se destina a alterar os revisores ou as decisões de uma revisão.  Para alterar os revisores, use as APIs [addReviewer](accessreview-addreviewer.md) [ou removeReviewer](accessreview-removereviewer.md) .  Para interromper uma revisão única já iniciada ou uma instância já iniciada de uma revisão recorrente, no início, use a API [de parada](accessreview-stop.md) . Para aplicar as decisões ao grupo de destino ou aos direitos de acesso do aplicativo, use a API [de aplicação](accessreview-apply.md) . 


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante)     | AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All |
|Delegada (conta pessoal da Microsoft) | Sem suporte. |
|Application                            | AccessReview.ReadWrite.Membership |

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
No corpo da solicitação, forneça uma representação JSON dos parâmetros de um [objeto accessReview](../resources/accessreview.md) .

A tabela a seguir mostra as propriedades que podem ser fornecidas quando você atualiza um accessReview.

| Propriedade      | Tipo           | Descrição                                                                                                |
|:--------------|:---------------|:-----------------------------------------------------------------------------------------------------------|
| displayName   | String         | O nome da revisão de acesso.                                                                                    |
| startDateTime | DateTimeOffset | O DateTime quando a revisão está agendada para ser iniciada.  Isso deve ser uma data no futuro.                 |
| endDateTime   | DateTimeOffset | O DateTime quando a revisão está agendada para terminar. Isso deve ser pelo menos um dia depois da data de início. |
| descrição   | Cadeia de caracteres         | A descrição, a ser mostrada aos revisores.                                                                 |



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `204 Accepted` de resposta e um [objeto accessReview](../resources/accessreview.md) no corpo da resposta.

## <a name="example"></a>Exemplo

Este é um exemplo de atualização de uma revisão de acesso única (não recorrente).

##### <a name="request"></a>Solicitação
No corpo da solicitação, forneça uma representação JSON das novas propriedades do [objeto accessReview](../resources/accessreview.md) .


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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-accessreview-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-accessreview-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
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


