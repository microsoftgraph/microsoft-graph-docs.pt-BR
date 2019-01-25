---
title: Aplicar accessReview
description: 'No Windows Azure AD para acessar o recurso de revisões, aplique as decisões de um accessReview concluída.  O objeto de destino pode ser uma revisão de acesso de uma única vez, ou uma instância de uma análise mais acesso recorrente.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9612f3bcb8a032ee32cd7b058d3f21950c9b120f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512210"
---
# <a name="apply-accessreview"></a>Aplicar accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, aplica as decisões de um concluídas [accessReview](../resources/accessreview.md).  O objeto de destino pode ser uma revisão de acesso de uma única vez, ou uma instância de uma análise mais acesso recorrente.  


Depois que uma revisão do access for concluída, um porque atingiu a data de término ou um administrador parou de manualmente e aplicar auto não foi configurado para a revisão, é possível chamar Apply para aplicar as alterações. Até aplicar ocorre, as decisões para remover os direitos de acesso não aparecem no recurso de código-fonte, os usuários por exemplo mantêm suas associações de grupo. Chamando aplicar, o resultado da revisão é implementado, atualizando o grupo ou o aplicativo. Se o acesso do usuário foi negado na revisão, quando um administrador chama este API, o Azure AD remove a atribuição de seus aplicativos ou da associação. 

Depois que uma revisão do access for concluída e aplicação de automática foi configurado, em seguida, o status da revisão deixará de ser concluído em estados intermediários e finalmente será alterado para o estado aplicado. Você deve esperar consulte negados users, se houver, que está sendo removido do recurso Agrupar atribuição de aplicativo ou associação em poucos minutos.

Um automático configurado a aplicação de revisão ou selecionando aplicar não tem efeito em um grupo que se origina de um diretório local ou um grupo dinâmico. Se você quiser alterar um grupo local de originado, baixe os resultados e aplicar essas alterações para a representação do grupo nesse diretório.


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | Token de portador Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.


## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.

## <a name="see-also"></a>Confira também

- [Como concluir uma revisão do access](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/applyDecisions()
```
##### <a name="response"></a>Resposta
>**Observação: **o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
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
    "Error: /api-reference/beta/api/accessreview-apply.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
