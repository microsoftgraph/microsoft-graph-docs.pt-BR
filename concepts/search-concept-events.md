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
# <a name="use-the-microsoft-search-api-to-search-calendar-events"></a><span data-ttu-id="c9f7e-103">Usar a API de pesquisa da Microsoft para pesquisar eventos de calendário</span><span class="sxs-lookup"><span data-stu-id="c9f7e-103">Use the Microsoft Search API to search calendar events</span></span>

<span data-ttu-id="c9f7e-104">Use a API de pesquisa da Microsoft para pesquisar eventos no calendário principal do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="c9f7e-104">Use the Microsoft Search API to search for events in the signed-in user’s primary calendar.</span></span> <span data-ttu-id="c9f7e-105">A identidade do usuário para a pesquisa se baseia no token de autenticação.</span><span class="sxs-lookup"><span data-stu-id="c9f7e-105">The user identity for the search is based on the auth token.</span></span>

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

## <a name="example"></a><span data-ttu-id="c9f7e-106">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c9f7e-106">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9f7e-107">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c9f7e-107">Request</span></span>

<span data-ttu-id="c9f7e-108">Este exemplo procura a palavra-chave "contoso" no calendário do usuário e retorna até 25 resultados.</span><span class="sxs-lookup"><span data-stu-id="c9f7e-108">This example searches in the user's calendar for the keyword "contoso", and will return up to 25 results.</span></span>

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

#### <a name="response"></a><span data-ttu-id="c9f7e-109">Resposta</span><span class="sxs-lookup"><span data-stu-id="c9f7e-109">Response</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="c9f7e-110">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="c9f7e-110">Known limitations</span></span>

- <span data-ttu-id="c9f7e-111">Você pode acessar somente a caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="c9f7e-111">You can access only the signed-in user’s own mailbox.</span></span> <span data-ttu-id="c9f7e-112">Não há suporte para a pesquisa de caixas de correio delegadas.</span><span class="sxs-lookup"><span data-stu-id="c9f7e-112">Searching delegated mailboxes is not supported.</span></span>
- <span data-ttu-id="c9f7e-113">Para eventos, a propriedade **total** do tipo [searchHitsContainer](/graph/api/resources/searchhitscontainer) contém o número de resultados na página, e não o número total de resultados correspondentes.</span><span class="sxs-lookup"><span data-stu-id="c9f7e-113">For events, the **total** property of the [searchHitsContainer](/graph/api/resources/searchhitscontainer) type contains the number of results on the page, not the total number of matching results.</span></span>
- <span data-ttu-id="c9f7e-114">A classificação de resultados não é suportada para eventos.</span><span class="sxs-lookup"><span data-stu-id="c9f7e-114">Sorting results is not supported for events.</span></span> <span data-ttu-id="c9f7e-115">Uma cláusula de classificação na solicitação retornará um código de erro de solicitação inválida na resposta.</span><span class="sxs-lookup"><span data-stu-id="c9f7e-115">A sort clause in the request will return a Bad Request error code in the response.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c9f7e-116">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="c9f7e-116">Next steps</span></span>

- [<span data-ttu-id="c9f7e-117">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="c9f7e-117">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview)
