---
title: Atualizar accessReview
description: No recurso de avaliações de acesso do Azure AD, atualize um objeto accessReview existente para alterar uma ou mais das suas propriedades.
localization_priority: Normal
ms.openlocfilehash: 65420b3682eb9d9f72d95beea624eb84429628ae
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833744"
---
# <a name="update-accessreview"></a>Atualizar accessReview

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

No recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, atualize um objeto [accessReview](../resources/accessreview.md) existente para alterar uma ou mais das suas propriedades.

Essa API não deve alterar os revisores ou decisões de uma revisão.  Para alterar os revisores, use o [addReviewer](accessreview-addreviewer.md) ou [removeReviewer](accessreview-removereviewer.md) APIs.  Para interromper uma revisão ocasional já iniciado ou uma instância já iniciado de uma revisão recorrente, no início, use o [Parar](accessreview-stop.md) API e para aplicar as decisões para os destino grupo ou app direitos de acesso, use a [Aplicar](accessreview-apply.md) API. 


## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /accessReviews('{reviewId}')
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | Portador \{token\}. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação de JSON dos parâmetros de um objeto [accessReview](../resources/accessreview.md) .

A tabela a seguir mostra as propriedades que podem ser fornecidas quando você atualiza um accessReview.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| `displayName`             |`String`                                                        | O nome de revisão de acesso.  |
| `startDateTime`           |`DateTimeOffset`                                                | DateTime quando a revisão está agendada para ser iniciar.  Isso deve ser uma data no futuro.   |
| `endDateTime`             |`DateTimeOffset`                                                | DateTime quando a revisão está agendada para terminar. Isto deve ser de pelo menos um dia mais recente do que a data de início.   |
| `description`             |`String`                                                        | A descrição, para mostrar aos revisores. |



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `204, Accepted` código de resposta e um objeto [accessReview](../resources/accessreview.md) no corpo da resposta.

## <a name="example"></a>Exemplo

Este é um exemplo de atualização de uma única revisão de acesso (não recorrentes).

##### <a name="request"></a>Solicitação
No corpo da solicitação, fornece uma representação JSON das novas propriedades do objeto [accessReview](../resources/accessreview.md) .

<!-- {
  "blockType": "request",
  "name": "update_accessReview"
}-->
```http
PATCH https://graph.microsoft.com/beta/accessReviews('006111db-0810-4494-a6df-904d368bd81b')
Content-type: application/json

{
    "displayName":"TestReview new name"
}
```

##### <a name="response"></a>Resposta
>**Observação: **o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
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
    "reviewerType": "delegate",
    "description": "Sample description"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Update accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
