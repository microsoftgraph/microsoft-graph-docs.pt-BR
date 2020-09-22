---
title: Usar a API de pesquisa da Microsoft no Microsoft Graph para pesquisar eventos de calendário
description: Você pode pesquisar no próprio calendário do usuário.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 802f6fdbb45d93ed46cd0b8033816abf5df07288
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48192592"
---
# <a name="use-the-microsoft-search-api-to-search-calendar-events"></a><span data-ttu-id="664f8-103">Usar a API de pesquisa da Microsoft para pesquisar eventos de calendário</span><span class="sxs-lookup"><span data-stu-id="664f8-103">Use the Microsoft Search API to search calendar events</span></span>

<span data-ttu-id="664f8-104">Use a API de pesquisa da Microsoft para pesquisar eventos no calendário principal do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="664f8-104">Use the Microsoft Search API to search for events in the signed-in user’s primary calendar.</span></span> <span data-ttu-id="664f8-105">A identidade do usuário para a pesquisa se baseia no token de autenticação.</span><span class="sxs-lookup"><span data-stu-id="664f8-105">The user identity for the search is based on the auth token.</span></span>

[!INCLUDE [search-schema-updated](../includes/search-schema-updated.md)]

## <a name="example"></a><span data-ttu-id="664f8-106">Exemplo</span><span class="sxs-lookup"><span data-stu-id="664f8-106">Example</span></span>

### <a name="request"></a><span data-ttu-id="664f8-107">Solicitação</span><span class="sxs-lookup"><span data-stu-id="664f8-107">Request</span></span>

<span data-ttu-id="664f8-108">Este exemplo procura a palavra-chave "contoso" no calendário do usuário e retorna até 25 resultados.</span><span class="sxs-lookup"><span data-stu-id="664f8-108">This example searches in the user's calendar for the keyword "contoso", and will return up to 25 results.</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
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

#### <a name="response"></a><span data-ttu-id="664f8-109">Resposta</span><span class="sxs-lookup"><span data-stu-id="664f8-109">Response</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#search",
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

## <a name="known-limitations"></a><span data-ttu-id="664f8-110">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="664f8-110">Known limitations</span></span>

- <span data-ttu-id="664f8-111">Você pode acessar somente a caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="664f8-111">You can access only the signed-in user’s own mailbox.</span></span> <span data-ttu-id="664f8-112">Não há suporte para a pesquisa de caixas de correio delegadas.</span><span class="sxs-lookup"><span data-stu-id="664f8-112">Searching delegated mailboxes is not supported.</span></span>
- <span data-ttu-id="664f8-113">Para eventos, a propriedade **total** do tipo [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta&preserve-view=true) contém o número de resultados na página, e não o número total de resultados correspondentes.</span><span class="sxs-lookup"><span data-stu-id="664f8-113">For events, the **total** property of the [searchHitsContainer](/graph/api/resources/searchhitscontainer?view=graph-rest-beta&preserve-view=true) type contains the number of results on the page, not the total number of matching results.</span></span>
- <span data-ttu-id="664f8-114">A classificação de resultados não é suportada para eventos.</span><span class="sxs-lookup"><span data-stu-id="664f8-114">Sorting results is not supported for events.</span></span> <span data-ttu-id="664f8-115">Uma cláusula de classificação na solicitação retornará um código de erro de solicitação inválida na resposta.</span><span class="sxs-lookup"><span data-stu-id="664f8-115">A sort clause in the request will return a Bad Request error code in the response.</span></span>

## <a name="next-steps"></a><span data-ttu-id="664f8-116">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="664f8-116">Next steps</span></span>

- [<span data-ttu-id="664f8-117">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="664f8-117">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
