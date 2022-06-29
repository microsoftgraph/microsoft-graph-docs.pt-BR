---
title: Usar a API de Pesquisa da Microsoft para pesquisar pessoas
description: Use a API de Pesquisa da Microsoft no Microsoft Graph para pesquisar pessoas relevantes para um usuário determinadas pelos padrões de comunicação e pelas relações comerciais do usuário.
author: acsehi
ms.localizationpriority: medium
ms.prod: search
ms.openlocfilehash: 3b1165a0bcac91ef7a74078b2d88fb268d0f40c6
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436194"
---
# <a name="use-the-microsoft-search-api-to-search-people"></a>Usar a API de Pesquisa da Microsoft para pesquisar pessoas

Os aplicativos do Microsoft Graph podem usar a API de Pesquisa da Microsoft para recuperar as pessoas mais relevantes para um usuário. A relevância é determinada pelos padrões de comunicação e colaboração e pelas relações comerciais do usuário. As pessoas podem ser contatos locais ou do diretório de uma organização ou pessoas de comunicações recentes.

Além de gerar esse insight, a pesquisa também fornece suporte à pesquisa de correspondência difusa e a capacidade de recuperar a lista de usuários relevantes para outro usuário na organização do usuário conectado.

## <a name="example-search-person-by-name"></a>Exemplo: Pesquisar pessoa por nome

A solicitação a seguir obtém as pessoas mais relevantes para o usuário conectado, com base em padrões de comunicação e colaboração e relações de negócios.

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

A seguir está um exemplo da resposta, que contém uma mensagem que corresponde ao critério de pesquisa.

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

- [Usar a API de Pesquisa da Microsoft para consultar dados](/graph/api/resources/search-api-overview)
