---
title: Adicionar Revisor accessReview
description: 'No recurso de avaliações de acesso do Azure AD, atualize um objeto accessReview existente para adicionar outro usuário como um revisor.  Essa operação só é permitida para uma revisão de acesso que ainda não foi concluída e apenas para uma revisão de acesso onde os revisores são explicitamente especificados. Essa operação não é permitida para uma revisão do access no qual os usuários revisam sua próprias acesso e não foi projetada para uma revisão de acesso na qual os proprietários do grupo são atribuídos como os revisores. '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1a526451330321c7fbbfd1d5287dd5ad892eee84
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516361"
---
# <a name="add-accessreview-reviewer"></a>Adicionar Revisor accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, atualize um objeto [accessReview](../resources/accessreview.md) existente para adicionar outro usuário como um revisor.  Essa operação só é permitida para uma revisão de acesso que ainda não foi concluída e apenas para uma revisão de acesso onde os revisores são explicitamente especificados. Essa operação não é permitida para uma revisão do access no qual os usuários revisam sua próprias acesso e não foi projetada para uma revisão de acesso na qual os proprietários do grupo são atribuídos como os revisores. 


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
POST /accessReviews('{reviewId}')/reviewers
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | Token de portador Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON da ID de um usuário que será um revisor.

A tabela a seguir mostra as propriedades que podem ser fornecidas quando você atualiza um accessReview.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| `id`             |`String`                                                        | ID do usuário.  |


## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201, Created` código de resposta.

## <a name="example"></a>Exemplo

Este é um exemplo de como atualizar uma revisão de acesso (não recorrentes) ocasional com um revisor adicional.

##### <a name="request"></a>Solicitação
No corpo da solicitação, fornece uma representação JSON da id do objeto de usuário.

<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/reviewers
Content-type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```

##### <a name="response"></a>Resposta
>**Observação: **o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created

```

<!--
{
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-addreviewer.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
