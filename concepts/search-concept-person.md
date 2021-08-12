---
title: Usar a API Pesquisa da Microsoft no Microsoft Graph pesquisar pessoas (visualização)
description: Você pode usar a API Pesquisa da Microsoft para pesquisar por pessoas relevantes para você.
author: acsehi
localization_priority: Normal
ms.prod: search
ms.openlocfilehash: ac978f09477db841e8f71a630128ba58d4f19ec2567813704a326ba49b13b818
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235090"
---
# <a name="use-the-microsoft-search-api-in-microsoft-graph-to-search-people-preview"></a>Usar a API Pesquisa da Microsoft no Microsoft Graph pesquisar pessoas (visualização)

Os Graph microsoft podem usar a API Pesquisa da Microsoft para recuperar as pessoas que são mais relevantes para um usuário. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário. As pessoas podem ser contatos locais ou do diretório de uma organização e pessoas de comunicações recentes. Juntamente com a geração desse insight, a pesquisa também fornece suporte à pesquisa de correspondência difusa e a capacidade de recuperar a lista de usuários relevantes para outro usuário na organização do usuário assinado.

## <a name="example-search-person-by-name"></a>Exemplo: Pessoa de pesquisa por nome

A solicitação a seguir obtém as pessoas mais relevantes para o usuário in-lo, com base nos padrões de comunicação e colaboração e relações comerciais.

### <a name="request"></a>Solicitação

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

### <a name="response"></a>Resposta

A seguir, um exemplo da resposta, que contém uma mensagem que corresponde ao critério de pesquisa.

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

## <a name="next-steps"></a>Próximas etapas

- [Usar a API Pesquisa da Microsoft de usuário](/graph/api/resources/search-api-overview)
