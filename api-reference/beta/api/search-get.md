---
title: Pesquisar
description: Recuperar o recurso de pesquisa usado para executar consultas
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 90db18f6dddeff1f3bf57b0f2c756928564d54f6
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703711"
---
# <a name="search"></a>Pesquisar

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso de pesquisa é o objeto de nível superior que representa o ponto de extremidade de pesquisa. Ela não se comporta como qualquer outro recurso no Graph, mas serve como uma âncora para ações de pesquisa (consulta). Ele não tem representação de recurso no gráfico.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Mail. Read, files. Read. All, Calendars. Read, ExternalItem. Read. All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
GET /search
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome      |Descrição|
|:----------|:----------|
| Autorização | Portador {token} |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Esse recurso não deve ser chamado como tal. Qualquer solicitação no recurso causará uma solicitação incorreta.

## <a name="next-steps"></a>Próximas etapas

- Explore a ação [/Query](search-query.md) na pesquisa.


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get search",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
