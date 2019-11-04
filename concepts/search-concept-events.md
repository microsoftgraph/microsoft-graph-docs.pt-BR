---
title: Eventos de calendário de pesquisa
description: Você pode pesquisar no próprio calendário do usuário.
author: knightsu
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: 1b749c0b45b8250d011589e20b05a3d715b40bcb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939555"
---
# <a name="search-calendar-events"></a><span data-ttu-id="3bb26-103">Eventos de calendário de pesquisa</span><span class="sxs-lookup"><span data-stu-id="3bb26-103">Search calendar events</span></span>

<span data-ttu-id="3bb26-104">Seu aplicativo pode no calendário principal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="3bb26-104">You app can in a user’s own primary calendar.</span></span> <span data-ttu-id="3bb26-105">A identidade do usuário usada para Pesquisar é baseada no token de autorização.</span><span class="sxs-lookup"><span data-stu-id="3bb26-105">The user identity used to search is based on the Authorization Token.</span></span>

## <a name="example"></a><span data-ttu-id="3bb26-106">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3bb26-106">Example</span></span>

### <a name="request"></a><span data-ttu-id="3bb26-107">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3bb26-107">Request</span></span>

<span data-ttu-id="3bb26-108">Este exemplo procura a palavra-chave "contoso" no calendário do usuário e irá recuperar até 25 resultados.</span><span class="sxs-lookup"><span data-stu-id="3bb26-108">This example searches in the user's calendar for the keyword "contoso", and will retrieve up to 25 results.</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json
```

```json
{
  "requests": [
    {
       "entityTypes": ["microsoft.graph.event"],
       "query": {
        "query_string": {
          "query": "contoso"
        }
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

## <a name="known-limitations"></a><span data-ttu-id="3bb26-109">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="3bb26-109">Known limitations</span></span>

<span data-ttu-id="3bb26-110">Você só pode acessar o próprio calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="3bb26-110">You can only access user’s own calendar.</span></span> <span data-ttu-id="3bb26-111">Não há suporte para o calendário compartilhado, acesso delegado.</span><span class="sxs-lookup"><span data-stu-id="3bb26-111">Shared Calendar, delegated access is not supported.</span></span>

## <a name="next-steps"></a><span data-ttu-id="3bb26-112">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="3bb26-112">Next steps</span></span>

<span data-ttu-id="3bb26-113">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="3bb26-113">Find out more about:</span></span>

- [<span data-ttu-id="3bb26-114">Usar a API de pesquisa</span><span class="sxs-lookup"><span data-stu-id="3bb26-114">Use the search API</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)