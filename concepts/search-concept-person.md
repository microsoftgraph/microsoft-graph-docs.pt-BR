---
title: Usar a API Pesquisa da Microsoft no Microsoft Graph pesquisar pessoas (visualização)
description: Você pode usar a API Pesquisa da Microsoft para pesquisar por pessoas relevantes para você.
author: acsehi
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: b9e53fadf7df205c315daf090350e7b4748b9025
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334812"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-people-preview"></a><span data-ttu-id="38fae-103">Usar a API Pesquisa da Microsoft no Microsoft Graph pesquisar pessoas (visualização)</span><span class="sxs-lookup"><span data-stu-id="38fae-103">Use the Microsoft Search API in Microsoft Graph to search people (preview)</span></span>

<span data-ttu-id="38fae-104">Os Graph microsoft podem usar a API de Pesquisa para recuperar as pessoas que são mais relevantes para um usuário.</span><span class="sxs-lookup"><span data-stu-id="38fae-104">Microsoft Graph applications can use the Search API to retrieve the people who are most relevant to a user.</span></span> <span data-ttu-id="38fae-105">A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="38fae-105">Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> <span data-ttu-id="38fae-106">As pessoas podem ser contatos locais ou do diretório de uma organização e pessoas de comunicações recentes.</span><span class="sxs-lookup"><span data-stu-id="38fae-106">People can be local contacts or from an organization’s directory, and people from recent communications.</span></span> <span data-ttu-id="38fae-107">Juntamente com a geração desse insight, a pesquisa também fornece suporte à pesquisa de correspondência difusa e a capacidade de recuperar a lista de usuários relevantes para outro usuário na organização do usuário assinado.</span><span class="sxs-lookup"><span data-stu-id="38fae-107">Along with generating this insight, search also provides fuzzy matching search support and the ability to retrieve the list of users relevant to another user in the signed in user's organization.</span></span>

## <a name="example-search-person-by-name"></a><span data-ttu-id="38fae-108">Exemplo: Pessoa de pesquisa por nome</span><span class="sxs-lookup"><span data-stu-id="38fae-108">Example: Search person by name</span></span>

<span data-ttu-id="38fae-109">A solicitação a seguir obtém as pessoas mais relevantes para o usuário assinado, com base nos padrões de comunicação e colaboração e relações comerciais.</span><span class="sxs-lookup"><span data-stu-id="38fae-109">The following request gets the people most relevant to the signed in user, based on communication and collaboration patterns and business relationships.</span></span>

### <a name="request"></a><span data-ttu-id="38fae-110">Solicitação</span><span class="sxs-lookup"><span data-stu-id="38fae-110">Request</span></span>

```HTTP
POST https://graph.microsoft.com/beta/search/query
Content-Type: application/json

{
  "requests": [
    {
      "entityTypes": [
        "person"
      ],
      "query": {
        "queryString": "contoso"
      },
      "from": 0,
      "size": 25
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="38fae-111">Resposta</span><span class="sxs-lookup"><span data-stu-id="38fae-111">Response</span></span>

<span data-ttu-id="38fae-112">A seguir, um exemplo da resposta, que contém uma mensagem que corresponde ao critério de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="38fae-112">The following is an example of the response, which contains one message that matches the search criterion.</span></span>

```HTTP
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://canary.graph.microsoft.com/testprodbetapersoninsearch/$metadata#microsoft.graph.searchResponse",
    "value": [
        {
            "hitsContainers": [
                {
                    "total": 1,
                    "moreResultsAvailable": false,
                    "hits": [
                        {
                            "hitId": "fc138b85-18ac-48e0-80a4-633ae4b594e0@41f988bf-86f1-53af-91ab-2d7cd034db47",
                            "rank": 1,
                            "summary": "",
                            "resource": {
                                "@odata.type": "#microsoft.graph.person",
                                "displayName": "Example User",
                                "givenName": "User",
                                "surname": "User",
                                "department": "Finance",
                                "officeLocation": "London",
                                "userPrincipalName": "example.user@contoso.com",
                                "emailAddresses": [
                                    {
                                        "address": "example.user@contoso.com",
                                        "rank": 1
                                    }
                                ],
                                "phones": [
                                    {
                                        "type": "business",
                                        "number": "+44 (20) 12345678"
                                    }
                                ]
                            }
                        }
                    ]
                }
            ]
        }
    ]
}
```

## <a name="next-steps"></a><span data-ttu-id="38fae-113">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="38fae-113">Next steps</span></span>

- [<span data-ttu-id="38fae-114">Usar a API Pesquisa da Microsoft de usuário</span><span class="sxs-lookup"><span data-stu-id="38fae-114">Use the Microsoft Search API</span></span>](/graph/api/resources/search-api-overview)
