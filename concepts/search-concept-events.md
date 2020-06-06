---
title: Usar a API de pesquisa da Microsoft no Microsoft Graph para pesquisar eventos de calendário
description: Você pode pesquisar no próprio calendário do usuário.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 6326fead96cd0b777ff6c3e257d6aa36d4d5c4ce
ms.sourcegitcommit: 093d89c7583bb6880c8395e9498a1f33cdd938b4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2020
ms.locfileid: "44568767"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-calendar-events"></a>Usar a API de pesquisa da Microsoft no Microsoft Graph para pesquisar eventos de calendário

Você pode usar a API de pesquisa da Microsoft para pesquisar eventos no calendário principal de um usuário. A identidade do usuário para a pesquisa se baseia no token de autenticação.

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este exemplo procura a palavra-chave "contoso" no calendário do usuário e retorna até 25 resultados.

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "entityTypes": [
        "event"
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

Você só pode acessar o próprio calendário do usuário. Não há suporte para o calendário compartilhado e o schenarios de acesso delegado.

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview?view=graph-rest-beta)
