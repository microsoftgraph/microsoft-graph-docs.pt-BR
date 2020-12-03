---
title: Usar a API de pesquisa da Microsoft no Microsoft Graph para pesquisar eventos de calendário
description: Você pode pesquisar no próprio calendário do usuário.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: bedad2dcf94df6024bcba7f0760dbe5c1cf97c18
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49521905"
---
# <a name="use-the-microsoft-search-api-to-search-calendar-events"></a>Usar a API de pesquisa da Microsoft para pesquisar eventos de calendário

Use a API de pesquisa da Microsoft para pesquisar eventos no calendário principal do usuário conectado. A identidade do usuário para a pesquisa se baseia no token de autenticação.

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Este exemplo procura a palavra-chave "contoso" no calendário do usuário e retorna até 25 resultados.

```HTTP
POST https://graph.microsoft.com/v1.0/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "event"
      ],
      "query": {
        "queryString":"contoso"
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

#### <a name="response"></a>Resposta

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#search",
  "value": [
  {
   "@odata.type": "#microsoft.graph.searchResponse",
   "searchTerms": [
    "contoso"
   ],
   "hitsContainers": [
    {
     "@odata.type": "#microsoft.graph.searchHitsContainer",
     "hits": [
      {
       "@odata.type": "#microsoft.graph.searchHit",
       "hitId": "AAMkADEwODY2NzllLTQ3MmEtNGRlMC05ZTUyLTE4ZDRhYmU1ZGM3NABGAAAAAAA3+iYQBnJnQabRVDelNhnzBwAejhWkAOAxQ6M4c1c9NwfrAAAAAAENAAAejhWkAOAxQ6M4c1c9NwfrAABbUZLJAAA=",
       "rank": 1,
       "summary": "Here is a summary of your events from last week",
       "resource": {
        "@odata.type": "#microsoft.graph.event",
        "end": {
         "dateTime": "2020-06-16T04:15:00Z",
         "timeZone": "UTC"
        },
        "hasAttachments": false,
        "iCalUId": "040000008200E00074C5B7101A82E008000000007093FDD79B3AD60100000000000000001000000036DAA2262EB4E04DA27DA77985FB8251",
        "isAllDay": false,
        "sensitivity": "Normal",
        "start": {
         "dateTime": "2020-06-16T03:30:00Z",
         "timeZone": "UTC"
        },
        "subject": "Weekly digest: Microsoft 365 changes",
        "type": "Single"
       }
      }
     ],
     "total": 1,
     "moreResultsAvailable": false
    }
   ]
  }
 ]
}
```

## <a name="known-limitations"></a>Limitações conhecidas

- Você pode acessar somente a caixa de correio do usuário conectado. Não há suporte para a pesquisa de caixas de correio delegadas.
- Para eventos, a propriedade **total** do tipo [searchHitsContainer](/graph/api/resources/searchhitscontainer) contém o número de resultados na página, e não o número total de resultados correspondentes.
- A classificação de resultados não é suportada para eventos. Uma cláusula de classificação na solicitação retornará um código de erro de solicitação inválida na resposta.

## <a name="next-steps"></a>Próximas etapas

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview)
