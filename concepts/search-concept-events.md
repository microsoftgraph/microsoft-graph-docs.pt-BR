---
title: Usar a API de pesquisa da Microsoft no Microsoft Graph para pesquisar eventos de calendário
description: Você pode pesquisar no próprio calendário do usuário.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: b7ea957419801c6e100412e5f46d2e1757387b3b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868524"
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

Você só pode acessar o próprio calendário do usuário. Não há suporte para o calendário compartilhado e o schenarios de acesso delegado.

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview?view=graph-rest-beta)
