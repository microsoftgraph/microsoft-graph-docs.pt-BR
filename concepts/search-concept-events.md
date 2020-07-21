---
title: Usar a API de pesquisa da Microsoft no Microsoft Graph para pesquisar eventos de calendário
description: Você pode pesquisar no próprio calendário do usuário.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 8cafb01337581d1b1d2e355363aec14f658ee4f6
ms.sourcegitcommit: 79267b6d78c3510ef609953c5a664e692794caaa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/21/2020
ms.locfileid: "45196824"
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

Você só pode acessar o próprio calendário do usuário. Não há suporte para cenários de acesso delegado e de calendário compartilhado.

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview?view=graph-rest-beta)
