---
title: Listar decisões accessReview
description: No recurso de revisões do Azure AD Access, recupere as decisões de um objeto accessReview.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 479699d55741830b542038dd43184a9ce7e1d535
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35440054"
---
# <a name="list-accessreview-decisions"></a>Listar decisões accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões do Azure AD [Access](../resources/accessreviews-root.md) , recupere as decisões de um objeto [accessReview](../resources/accessreview.md) .

Observe que uma revisão de acesso recorrente não terá uma `decisions` relação.  Em vez disso, o chamador deve `instance` navegar na relação para `accessReview` localizar um objeto para uma instância atual ou passada da revisão do Access.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview. Read. All, AccessReview. ReadWrite. All  |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | AccessReview.Read.All |

 O usuário conectado também deve estar em uma função de diretório que permite que ele leia uma revisão do Access.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Nenhum corpo de solicitação deve ser fornecido.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200, OK` um código de resposta e uma matriz de objetos [accessReviewDecision](../resources/accessreviewdecision.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação


# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objetivo-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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

## <a name="see-also"></a>Confira também

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter accessReview](accessreview-get.md) |  [accessReview](../resources/accessreview.md) |  Recupere uma revisão do Access. |
|[Listar minhas decisões do accessReview](accessreview-listmydecisions.md) |        coleção [accessReviewDecision](../resources/accessreviewdecision.md)|    Como revisor, obtenha as minhas decisões de um accessReview.|
|[Enviar lembrete accessReview](accessreview-sendreminder.md) |       Nenhum.   |   Envie um lembrete para os revisores de um accessReview. |
|[Parar accessReview](accessreview-stop.md) |        Nenhum.   |   Parar um accessReview. |
|[Redefinir decisões do accessReview](accessreview-reset.md) |        Nenhum.   |   Redefina as decisões em um accessReview em andamento.|
|[Aplicar decisões accessReview](accessreview-apply.md) |        Nenhum.   |   Aplique as decisões de um accessReview concluído.|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
