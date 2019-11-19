---
title: Eventos de calendário de pesquisa
description: Você pode pesquisar no próprio calendário do usuário.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 2db61462670a553376467cf2329d26cbb339c452
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703971"
---
# <a name="search-calendar-events"></a>Pesquisar eventos do calendário

Seu aplicativo pode no calendário principal de um usuário. A identidade do usuário usada para Pesquisar é baseada no token de autorização.

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este exemplo procura a palavra-chave "contoso" no calendário do usuário e irá recuperar até 25 resultados.

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "microsoft.graph.event"
      ],
      "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

## <a name="known-limitations"></a>Limitações conhecidas

Você só pode acessar o próprio calendário do usuário. Não há suporte para o calendário compartilhado, acesso delegado.

## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Usar a API de pesquisa](/graph/api/resources/search-api-overview?view=graph-rest-beta)
