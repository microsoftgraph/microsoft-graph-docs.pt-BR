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
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-calendar-events"></a><span data-ttu-id="a8363-103">Usar a API de pesquisa da Microsoft no Microsoft Graph para pesquisar eventos de calendário</span><span class="sxs-lookup"><span data-stu-id="a8363-103">Use the Microsoft Search API in Microsoft Graph to search calendar events</span></span>

<span data-ttu-id="a8363-104">Você pode usar a API de pesquisa da Microsoft para pesquisar eventos no calendário principal de um usuário.</span><span class="sxs-lookup"><span data-stu-id="a8363-104">You can use the Microsoft Search API to search for events in a user’s primary calendar.</span></span> <span data-ttu-id="a8363-105">A identidade do usuário para a pesquisa se baseia no token de autenticação.</span><span class="sxs-lookup"><span data-stu-id="a8363-105">The user identity for the search is based on the auth token.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="example"></a><span data-ttu-id="a8363-106">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a8363-106">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8363-107">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8363-107">Request</span></span>

<span data-ttu-id="a8363-108">Este exemplo procura a palavra-chave "contoso" no calendário do usuário e retorna até 25 resultados.</span><span class="sxs-lookup"><span data-stu-id="a8363-108">This example searches in the user's calendar for the keyword "contoso", and will return up to 25 results.</span></span>

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

## <a name="known-limitations"></a><span data-ttu-id="a8363-109">Limitações conhecidas</span><span class="sxs-lookup"><span data-stu-id="a8363-109">Known limitations</span></span>

<span data-ttu-id="a8363-110">Você só pode acessar o próprio calendário do usuário.</span><span class="sxs-lookup"><span data-stu-id="a8363-110">You can only access user’s own calendar.</span></span> <span data-ttu-id="a8363-111">Não há suporte para o calendário compartilhado e o schenarios de acesso delegado.</span><span class="sxs-lookup"><span data-stu-id="a8363-111">Shared calendar and delegated access schenarios are not supported.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a8363-112">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a8363-112">Next steps</span></span>

- [<span data-ttu-id="a8363-113">Usar a API de Pesquisa da Microsoft para consultar dados</span><span class="sxs-lookup"><span data-stu-id="a8363-113">Use the Microsoft Search API to query data</span></span>](/graph/api/resources/search-api-overview?view=graph-rest-beta)
