---
title: Aplicar accessReview
description: 'No recurso de revisões de acesso do Azure AD, aplique as decisões de um accessReview concluído.  O objeto de destino pode ser uma revisão de acesso único ou uma instância de uma revisão de acesso recorrente.  '
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: b590b741915aaf9ef901ee51e2eb11d43f9b439f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048530"
---
# <a name="apply-accessreview"></a>Aplicar accessReview

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso de revisões de acesso do Azure [AD,](../resources/accessreviews-root.md) aplique as decisões de um [accessReview concluído.](../resources/accessreview.md)  O objeto de destino pode ser uma revisão de acesso único ou uma instância de uma revisão de acesso recorrente.  


Depois que uma revisão de acesso for concluída, porque ela atingiu a data de término ou um administrador a interrompeu manualmente e a aplicação automática não foi configurada para a revisão, você pode chamar Apply para aplicar as alterações. Até que ocorra a aplicação, as decisões para remover direitos de acesso não aparecem no recurso de origem, os usuários, por exemplo, retêm suas associações de grupo. Ao chamar aplicar, o resultado da revisão é implementado atualizando o grupo ou aplicativo. Se o acesso de um usuário foi negado na revisão, quando um administrador chama essa API, o Azure AD remove sua atribuição de associação ou aplicativo. 

Depois que uma revisão de acesso for concluída e a aplicação automática tiver sido configurada, o status da revisão mudará de Concluído para estados intermediários e, finalmente, mudará para o estado Aplicado. Você deve esperar ver usuários negados, se algum, sendo removidos da associação do grupo de recursos ou atribuição de aplicativos em alguns minutos.

Uma revisão automática configurada ou selecionar Aplicar não tem efeito em um grupo que se origina em um diretório local ou em um grupo dinâmico. Se você quiser alterar um grupo que se origina no local, baixe os resultados e aplique essas alterações à representação do grupo nesse diretório.


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.ReadWrite.Membership, AccessReview.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Application                            | AccessReview.ReadWrite.Membership |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/applyDecisions
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | \{token\} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.


## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/applyDecisions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/apply-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/apply-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/apply-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/apply-accessreview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Apply accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

## <a name="see-also"></a>Confira também

- [Como concluir uma revisão de acesso](/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)
