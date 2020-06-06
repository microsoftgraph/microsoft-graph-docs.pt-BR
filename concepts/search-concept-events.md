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
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-calendar-events"></a><span data-ttu-id="4b4d2-103">Usar a API de pesquisa da Microsoft no Microsoft Graph para pesquisar eventos de calendário</span><span class="sxs-lookup"><span data-stu-id="4b4d2-103">Use the Microsoft Search API in Microsoft Graph to search calendar events</span></span>

<span data-ttu-id="4b4d2-104">Você pode usar a API de pesquisa da Microsoft para pesquisar eventos no calendário principal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4b4d2-104">You can use the Microsoft Search API to search for events in a user’s primary calendar.</span></span> <span data-ttu-id="4b4d2-105">A identidade do usuário para a pesquisa se baseia no token de autenticação.</span><span class="sxs-lookup"><span data-stu-id="4b4d2-105">The user identity for the search is based on the auth token.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="example"></a><span data-ttu-id="4b4d2-106">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4b4d2-106">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b4d2-107">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4b4d2-107">Request</span></span>

<span data-ttu-id="4b4d2-108">Este exemplo procura a palavra-chave "contoso" no calendário do usuário e retorna até 25 resultados.</span><span class="sxs-lookup"><span data-stu-id="4b4d2-108">This example searches in the user's calendar for the keyword "contoso", and will return up to 25 results.</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="4b4d2-109">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="4b4d2-109">Known limitations</span></span>

<span data-ttu-id="4b4d2-110">Você só pode acessar o próprio calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="4b4d2-110">You can only access user’s own calendar.</span></span> <span data-ttu-id="4b4d2-111">Não há suporte para o calendário compartilhado e o schenarios de acesso delegado.</span><span class="sxs-lookup"><span data-stu-id="4b4d2-111">Shared calendar and delegated access schenarios are not supported.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4b4d2-112">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="4b4d2-112">Next steps</span></span>

- [<span data-ttu-id="4b4d2-113">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="4b4d2-113">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
